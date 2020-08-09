# 使用Qiskit学习量子计算

欢迎来到Qiskit社区! 本电子书是大学量子算法或计算课程基于Qiskit的学习附加资:

* 量子背后的数学
* 在IBM云量子系统上的量子算法

## 从这里开始

运行服务器之前,　你需要在电脑上安装 Node.js 和 NPM. 按照 [官方页面](https://nodejs.org)上的指导安装.

 forking 并克隆本仓库后, 用命令 `npm install`安装所有的依赖包.

现在你可以运行`npm start`命令开启本地服务.等待资产编译后打开[localhost:5000](http://localhost:5000).服务器将自动监听到文件的文件变化.


## 课程机构

每个课程都是在[content](content)目录下的文件夹.每个课程由下面不同组件组成:

* `content.md` 包含课程资源代码和数据. 它由[custom
  extension](https://mathigon.io/markdown)  [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)格式写成.
* `functions.ts` 包含所有课程指定的TypeScript代码.
* `styles.less` 包含所有课程指定的styles, 为[LESS](http://lesscss.org/)格式.
* `hints.yaml` (可选)包含由Mathigon之虚拟个人家教传达的任何信息.

[共享目录](content/shared)包含多课程使用人物传记、专业术语和课程资产.

每个课程分为若干步骤,每一步带有唯一的ID. 这些ID在`functions.ts`当每节函数输出借口时被使用到.　每个函数获得一个名为`$step`的参数,相应步骤在第一时间被解析到.在文件[types.d.ts](content/shared/types.d.ts)有可供使用的性质与方法，可查看使用之.
