# wiki.zhgdg.org

- 基于 markdoc 
- 通过 7niu CDN
- 发布所有 blog.zhgdg.org 的文章

## 进展

- 141228 ZQ 追加使用 gitcafe-pages 服务
    + 在 master 分支中进行 wiki 内容维护
    + 配置 `markdoc.yaml` 中 `html-dir: ".html"`
    + 配合 `fab p2cafe` 完成自动发布
    + 即, 使用项目 `pages` 服务,通过 `gitcafe-pages` 分支,将编译后的 html 文件发布为网站
- 141218 ZQ re-pub
