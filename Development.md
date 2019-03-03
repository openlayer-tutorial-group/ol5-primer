# 教程编写说明
---- 
## 1. 首要说明
* 首要申明：教程组的所有成员是一个团队，而不是团体，**相互尊重，相互帮助，团结共进**。
* 作为一本入门教程，**责任重大**，团队所有成员应竭尽全力确保教程内容**准确无误**，切忌误人子弟。
* 作为一本入门教程，理应做到**简洁明了，通俗易懂**，凡是能达成该目的所有技术手段和呈现方式都值得提倡。
## 2. 注意事项
* 请尽量使用中文，专业术语除外，比如OpenLayers，WMTS，TMS等
* 本教程采用GitBook工具来生成教程，在参与教程编写之前，请先自行学习了解GitBook，Markdown的相关知识（可参见[GitBook 使用教程][1]和[Markdown语法][2]）。 
* GitBook适配的Node版本要小于等于6，否则不行。
## 3. 编写规范
* 教程编写采用认领制，具体参见下面的认领制度。
* 编写时，请先Fork项目，在Fork出来的项目中编写，然后PR到本项目。经过团队两人以上的Review通过后，方能合入。
* 如果因为有事不能如期完成认领任务，需要反馈给我们的Master，并提交自己完成的部分，方便后续其他认领者接着做。如果过期没完成，也没有反馈，我们将会直接征求其他同学来认领，以保障整个教程持续下去。
* 目录结构规范：
	* 教程相关的信息都在contents目录里面;
	* 相关章节的文档都按照章节放在contents/chxxx目录下；
	* 文件命名按照章节编号命名，并遵循层级目录结构。例如：第一章的主页面命名为contents/ch01/ch01.md，第一章第一节页面命名为contents/ch01/ch01-01.md，第一章第一节下面的第一节页面命名为contents/ch01/ch01-01-01.md，以此类推；
	* 用到的示例代码统一放在contents/codes下面，并按照文档目录结构存放；
	* 图片统一放在contents/images下面，并按照文档目录结构存放；
* 在文档中添加示例代码，统一使用GitBook插件include-codeblock引入展示，插件已配置好，仅需要在编写文档时，用[import](path/document.md)来引入，更详细的语法参见[include-codeblock插件主页][3]
## 4. 认领制度流程
* 认领前请查看最新目录章节的认领情况，选择未认领的章节进行认领。
* 通过在企划群里面发消息（认领的章节及详细时间周期）给SM申请认领。
* 团队讨论确认后，回复消息给认领人，通知认领成功与否。
* 认领成功后，目录章节会更新认领情况。
## 5. 交流工具
* 目前采用QQ群进行沟通协作，有问题及需要都可以加入QQ群693790689。
* 有任何和教程相关的问题，可以在群里找我们的ScrumMaster，或者管家，ScrumMaster和管家在群名片都有备注。
## 6. GitBook环境简要搭建
* 安装node v6的版本和对应的npm。
* 执行命令`npm install -g gitbook-cli`安装对应的命令行工具。
* 进入目录contents。
	* 执行命令`gitbook init`进行初始化。
	* 执行命令`gitbook install`安装相应的插件。
	* 执行命令`gitbook build`进行构建。
	* 执行命令`gitbook server`启动服务，在浏览器访问[http://localhost:4000][4]即可看到教程页面。


[1]:	https://www.jianshu.com/p/421cc442f06c
[2]:	http://gitbook.hushuang.me/syntax/markdown.html
[3]:	https://plugins.gitbook.com/plugin/include-codeblock
[4]:	http://localhost:4000