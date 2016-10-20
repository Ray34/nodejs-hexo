---
title: Hexo+Github制作我的博客
tags: 
    - hexo
    - next
---
搭建基于Hexo+Github的博客已经有段时间了，第一篇文章一直没写，具体的配置步骤忘的差不多，下面是之前参考的一个博客：

[HEXO搭建个人博客](http://baixin.io/2015/08/HEXO%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2/).

### 常用命令

```bash
hexo clean
hexo generate
hexo deploy
```

### 遇到问题总结 

1、在修改_config.yml文件时，注意type: git冒号后面一定要有空格，其他几个也一样。
2、使用next主题时，修改headband的背景颜色：
    - 修改next/source/css/_schemes/_variables/base.styl第210行的$headband-bg和第224行的$brand-bg；
    - 相同路径Mist/Muse/Pisces文件夹下面的_brand.styl的第四行backgroud属性；

3、文章添加标签方法

```bash
tags:
  - tag1
  - tag2
```

4、[创建标签云页面](https://github.com/iissnan/hexo-theme-next/wiki/%E5%88%9B%E5%BB%BA%E6%A0%87%E7%AD%BE%E4%BA%91%E9%A1%B5%E9%9D%A2)
5、[next主题使用手册](http://theme-next.iissnan.com/getting-started.html#download-next-theme)