# PHP 开发者实践
PHP Developer Prepares

坚持了5年的创业项目决定结束了（行业垂直搜索方向，理想很美好、现实很骨感），作为 2000 年那波没混好的草根站长 & 09年这波没被风吹起来的小型互联网公司的技术合伙人，个人基本见证了这几年 PHP 环境的发展（当然主要归功于互联网创业项目的大爆发），感受了一些 PHP 团队和从业者的现状；同时，我们自身在 PHP 研发团队组建过程中也遇到了不少问题，一直想把创业过程中遇到的这些团队实践相关问题整理、总结一下，不过，完美主义(重度拖延症患者)害死人。。。

春节转眼刷完了，痛定思痛，又逢娃哭的厉害（夜哭郎。。。谁带谁知道 :-( ），小爆一夜，算是搞了个初始版本出来，欢迎大家拍砖 & 加入！

技术的发展日新月异，我会持续维护、跟进这个项目，欢迎各位有兴趣的朋友 [提交建议、问题 - Issue](https://github.com/zacao/php-developer-prepares/issues) 或 [贡献、分享 - Pull Request](https://github.com/zacao/php-developer-prepares/pulls)。本项目在 Github 上维护，欢迎参与：[https://github.com/zacao/php-developer-prepares](https://github.com/zacao/php-developer-prepares)。

***

近年来，越来越多的 Web 开发人员投入 Python, Node.js, Ruby 的怀抱，与此同时 PHP 也越来越多被人诟病，尽管 PHP 仍然是目前使用最广泛、重要的 Web 开发语言之一。经过几年观察，我发现造成国内这一奇怪现象的原因很大程度上是由于近几年市场对 PHP 开发人员井喷式需求导致大量未经良好训练的 PHP 新兵涌入、原有 PHP 老人多是站长出身且知识结构又未能及时与近几年 PHP 社区更新同步、大量基于原有实践开发的开源项目影响等因素的多重叠加。不论将来后端语言谁是最后的王者，至少在近段时间内 LA/NMP(Linux, Apache/Nginx, MySQL, PHP) 技术仍然是众多中小互联网创业公司的首选技术栈之一，我们尝试在新项目开发过程中更好的使用 PHP 技术，通过结合国外 PHP 领域最新的开发模式、工具和经验，使您的 PHP 项目、团队焕发新生，重装上阵。

  * 本文排版遵循 [文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines) 规范
  * 开发过程中遇到的绝大多数问题实际上都可以通过搜索引擎找到，关于搜索引擎使用技巧，请参考  [如何用好 Google 等搜索引擎？](http://www.zhihu.com/question/20161362)
  * 开发过程中遇到问题在论坛、社区中提问也是很常见的情况，如何尽可能让自己得到满意的答复，请参考 [提问的智慧 - English](http://www.catb.org/~esr/faqs/smart-questions.html) 或 [提问的智慧 - 中文](http://www.beiww.com/doc/oss/smart-questions.html)
  * 因为关于如何使用 PHP 语言本身相关资料已有很多，本文将尽量不涉及 PHP 语言本身并优先引用现有资料，主要围绕关心 PHP 项目开发技巧和具体实践，通过相关工具和经验的分享，大家在项目中更好的使用 PHP 技术。


## 在线阅读

 * http://ryancao.gitbooks.io/php-developer-prepares/content/

> 重要说明：正在持续修改之中，大部分章节都没有写完，正式发布还需要一段时间，所有内容随时可能发生变动。

## 如何参与

* 在 GitHub 上把本项目 `fork` 到自己的仓库，如 `<your-username>/php-developer-prepares`，然后 `clone` 到本地，并设置用户信息。
```
$ git clone git@github.com:<your-username>/php-developer-prepares.git
$ cd php-developer-prepares
$ git config user.name "yourname"
$ git config user.email "your email"
```
* 修改代码后提交，并推送到自己的仓库。
```
$ #do some change on the content
$ git commit -am "Fix issue #1: change helo to hello"
$ git push
```
* 在 GitHub 网站上提交 pull request。
* 定期使用项目仓库内容更新自己仓库内容。
```
$ git remote add upstream https://github.com/zacao/php-developer-prepares
$ git fetch upstream
$ git checkout master
$ git rebase upstream/master
$ git push -f origin master
```


## 授权许可

本文采用创意共享 [「署名-非商业性使用」](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh) 许可证（Creative Commons Attribution-NonCommercial license）。所有内容不仅可以免费阅读，还可以自由使用（比如转载），只需遵守两个条件：

- **署名**：必须保留原作者的署名。

- **非商业性使用**：除非得到正式许可，否则不得用于商业目的。