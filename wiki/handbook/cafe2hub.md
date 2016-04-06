# gitcafe 2 GitHub

[TOC]

## bg.
![404 gitcafe forever](http://zoomq.qiniudn.com/ZQCollection/snap/404-500/404_gitcafe_160401.png?imageView2/2/w/420)


## processing

![gh_pages_settings](http://zoomq.qiniudn.com/ZQCollection/snap/pages/gh_pages_settings.png?imageView2/2/w/420)

如果见到以上提示, 说明一切 `安好` ;-)

### UserName/Organization site

https://github.com/DevRela/devrela.github.io

这种比较简单:

- 追加 `CNAME` ~ `devrel.info`
- DNSPod 修订 CNAME
    + `@` ~ `devrela.github.io`
- `KO`

### Project site

https://github.com/zoom-quiet/wiki

这种,也就多一步:

- 建立分支 `git co -b hg_pages`
- 复制为 `output` 目录
- 定制 `fab` 事务 ~ [wiki/fabfile.py at master · zoom-quiet/wiki](https://github.com/zoom-quiet/wiki/blob/master/fabfile.py#L44)
    + 自动化这么几件事儿:
        * 用 `markdoc` 工具编译
        * 将 `CNAME` 复制到 `output`
        * 切换到 `output` 中将新编译结果用 `git` 命令推送到 github
- 思路上参考: [jekyll-to-pelican | #是也乎# | ZoomQuiet.io](http://blog.zoomquiet.io/jekyll-to-pelican.html)


## points
~ 最关键的几点

### DNSPod

- 使用一致的快速简洁的域名配置管理界面非常节省心力
- DNSPod 的确是国内用户首选

### coding

- 这次 gitcafe 合并入 coding 是好事儿
- 但是, pages 服务毕竟不是 coding 的核心业务
- 参考: [Coding 演示平台](http://docs.coding.io/)
    + 其操作/自动化 都非常初级
    + 和 gitcafe 当初的配置界面实在无法相比

![404 gitcafe pages](http://zoomq.qiniudn.com/ZQCollection/snap/404-500/404_gitcafe_pages.png?imageView2/2/w/420)

果断弃疗 ;-( 

### ghp-import
~ [ghp-import](https://github.com/davisp/ghp-import)

神器! 配合 pelican 的静态网站发布更加简洁


## (￣▽￣)

- 160406 大妈 记要
- 160401 大妈 启动

