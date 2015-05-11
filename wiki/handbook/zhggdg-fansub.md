# 珠海 GDG 字幕组工作流程

[TOC]

## 背景

## 分析

[珠海 GDG 学生贡献奖状获得规章](zhggdg-goa)

## 方案

## 进展
中国GDG字幕组的开源项目式协同流程

背景：
GDG字幕组官方网站 
http://www.gfansub.com/

GDG字幕组翻译最佳实践 - Google 文档
https://www.gdgdocs.org/document/d/1ZLp0U-Fm4q2Msbdtx8_0EHQRZiI6qQmvBQ_L0zHbLc0/edit

我是一名来自珠海的GDGer，现在是GDG字幕组(NanYang)的翻译人员。
但是GDG字幕组翻译流程过长，不能够及时把最新最酷的科技分享到互联网上供中国的开发者们学习。
作为一个热爱Google技术的GDGer，我决定改变这个现状。
于是GDG字幕组的开源项目式协同流程应运而生。

分析：
全程透明 ~ 全部有可接触的服务来公开
基本自主 ~ 全部基于 github 协同工作流来主动推进不需要过多的专职人员来管理

方案：
###技术翻译人员工作流程
- 项目规范
    + 仓库中创建对应视频名的文件夹，文件夹包含字幕文件，说明文件。字幕文件为字幕内容，说明文件为视频地址，参与项目者可根据规范自行创建项目并编写项目内容

- 流程

注册Github帐号
Fork项目

# 克隆fork后的项目
git clone https://github.com/yourgithubname/gfansub

# 添加上游仓库
git remote add upstream https://github.com/ZHGDG/gfansub 

# 提交本地修改
git add 被修改文件
git commit -m "****"  //***为修改内容注释
git push origin master

# pull request
在自己Github项目仓库下提交pull request到上游仓库

# 同步上游版本
git remote update upstream
git rebase upstream/master
git push origin master

管理员只做一件事情，merge request，merge的时候要判断内容的准确性以及对质量的把控

###非技术翻译人员工作流程
注册Github帐号
Fork项目

- 打开要翻译的文档，点击右上角的笔”Edit this file”进行翻译
- 翻译完成之后添加描述，然后点击下方的”Commit changes”进行保存
- 点击文本框右边第二个按钮”Pull requests”进行提交
- 等待管理员确认

进展：
# Github仓库
https://github.com/ZHGDG/gfansub

# 中国GDG字幕组专用MailList
zhgdgsubtitle@googlegroups.com
https://groups.google.com/forum/#!forum/zhgdgsubtitle

福利：
    1.小伙伴们通过翻译得来的知识是天然福利 XD
    2.拥有对自己的翻译的署名权，毕竟是劳动成果嘛 :)
    3.通过翻译字幕，你们可以认识来自全国各地的小伙伴们，拓展自己的社交圈

参考：
# 珠海GDG 社区文章撰写指南 
http://blog.zhgdg.org/2014-09/gdg-writer-guider/
# Fork+Pull工作模式-GotGitHub
http://www.worldhello.net/gotgithub/04-work-with-others/010-fork-and-pull.html
# 知识共享WiKi
http://zh.wikipedia.org/wiki/%E5%88%9B%E4%BD%9C%E5%85%B1%E7%94%A8



## 参考

- 150511 大妈 整理 Martin 草案发布


