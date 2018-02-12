# PPDAI开源项目贡献指南


## 欢迎 Welcome

非常欢迎您加入PPDI开源项目！我们非常感激您对项目的任何贡献，这些贡献包括但不限于，
- 报告项目的问题。
- 建议项目进行开发的新功能。
- 对项目贡献代码。
- 其它，比如参与项目讨论、发表建设性的看法等等。

下面将对如何进行这几个方面的流程指南进行介绍。

## 贡献者须知 Before Get Started
为了维护更好的开源社区环境，我们希望所有贡献者阅读并遵守参与者公约（code-of-conduct），
- 英文版：[code-of-conduct v1.4](https://www.contributor-covenant.org/version/1/4/code-of-conduct.html)
- 中文版：[参与者公约 v1.4](https://www.contributor-covenant.org/zh-cn/version/1/4/code-of-conduct.html)

## 报告问题 Report A Bug
我们通过Github的项目Issues列表跟踪所有发现的问题，在准备报告问题之前，你可以查看是否该问题在列表中，Github上有提供对issue的过滤查询，方便查找。

若没有找到或者不确定是否已有，你可以先创建一个Issue。任何Issue包括一个标题和内容，若能提供清晰和详细的问题描述，将会有助于问题的沟通和定位解决。

## 建议新功能 Suggest A Feature
我们通过Github的项目Issues列表跟踪用户对项目的新功能期望和建议。

若你对当前项目功能有特别期待的功能，请通过Github的项目Issues列表报告，在Issue的标题中请以“【新功能】”开头描述，这以便区分问题（bug）和功能（feature）。

## 贡献代码 Contribute Code
我们通过PR（Pull Request）的方式进行贡献代码的合并，对于整个PR流程可以参考Kubernates的社区开发指导，
- [Kubernates community - contribute guide - github workflow](https://github.com/kubernetes/community/blob/master/contributors/guide/github-workflow.md)

关于什么PR？一个简单的PR介绍请见[这里](https://help.github.com/articles/about-pull-requests/)。

在尽可能的情况下，让一个PR和一个Issue进行一一对应，换句话说，一个PR修复了一个Issue的报告问题，或者开发了一个Issue建议的新功能。

为了方便贡献代码，也为了保证开源代码的可持续性维护和开发，在提交PR前，请按照如下步骤步骤进行贡献代码，
- 在项目Issue列表中，选择一个Issue，将其分派给自己。
- Fork出项目代码仓库到自己账号中。
- 对这个Issue在fork出来上的仓库进行开发/修复。
- 运行单元测试、功能验收测试和相关其它测试，直到全部通过。
- 检查代码命名风格和注释。
- 提交commit，commit的信息尽量简单有意义，可参考此文[How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)。
- 提交一个PR，PR的正文格式范文见下面。

```
## 描述
这是一个PR提交的正文格式范文

## 修复/开发的Issue
Issue #1 - 没有进行Null检查...

## 讨论前后背景（若有）

## 代码更新类别
<!--- 选择一个代码更新类别? 在符合的类别方框[ ]中填入`x` -->
- [ ] 修复Bug （不改变当前已有的任何功能，在修复问题时）
- [ ] 新功能 New feature （不改变当前已有的任何功能，在新增该功能时）
- [ ] 改变已有功能 （当前的PR可能会改变已有功能）

## 检查列表
- [ ] 我已阅读HOW-CONTRIBUTE文档
- [ ] 代码风格和注释检查
- [ ] 单元测试通过
- [ ] 验收测试通过
- [ ] 其它测试通过（若有）
- [ ] 当前代码变化需要更新文档
- [ ] 文档已根据当前代码变化进行更新

## 其它信息（若有）

```
若一切准备就绪，那么提交PR吧，在那里我们进行code review和代码合并，若一切顺利，您贡献的代码将正式进入项目中。

再次感谢您对项目的努力和贡献！

## 其它问题 Other Issue
有更多问题，欢迎通过项目的Issue列表报告并讨论。

注：我们不推荐邮件联系的方式对问题进行讨论，因为邮件的讨论方式比较局限在部分人之间沟通，不便其他人获取信息和后续跟踪。
