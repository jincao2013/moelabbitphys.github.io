# Lab MOE BIT phys

This is a static website of moe lab for department of physics of Beijing institute of technology. 


### 文件结构

qfmda.com的全部文件的目录结构：

```Bash
jindeiMac:website.moelabbitphys jincao% pwd
/Volumes/jindedata/jindedata.bitphyswebdev/website.moelabbitphys
jindeiMac:website.moelabbitphys jincao% tree -L 2
.
├── resouce
│   ├── afdesign # 一些网址上用到的平面设计
│   ├── doc\ from\ biyue
│   ├── doc\ from\ liyuanchang
│   ├── doc\ from\ majie
│   └── science_lab.zip
└── src # 网址的源代码
    ├── archive # 以.tar.gz格式发布的源代码
    ├── backup # 以前的代码
    └── moelabbitphys # 当前网址的源代码
```



`src/qfmda` 的目录结构

```Bash
jindeiMac:moelabbitphys jincao% pwd
/Volumes/jindedata/jindedata.bitphyswebdev/website.moelabbitphys/src/moelabbitphys
jindeiMac:moelabbitphys jincao% tree -L 1 -a
.
├── .git
├── .gitignore # 指定哪些文件不属于git
├── .idea # webstorm 的配置文件，已在gitignore里面屏蔽
├── README.md
├── about.html
├── contact.html
├── fonts
├── images
├── index.html
├── interCommu.html
├── js
├── labedu.html
├── peoples.html
├── project.html
├── projects.html
├── research.html
├── sass
└── style.css

6 directories, 13 files
```



### 如何修改网页内容

参考 qfmda.com 的README.md



### 如何部署网址

参考 qfmda.com 的README.md



### 常用git命令

``` Bash
git clone https://e.coding.net/quantumlab/qfmda/qfmda.git # 克隆远程库到本地

git add * # 添加文件到暂存区。
git commit -m "" # 将暂存区内容添加到仓库中。
git push origin master # 把当前master分支推送到远程服务器origin

git fetch origin master:master # 把远程仓库origin的master分支拉回到本地的master分支，如果是Fast-forward就执行合并，如果有冲突则不合并
git merge FETCH_HEAD # 合并origin/master到工作区

git remote set-url origin https://e.coding.net/quantumlab/qfmda/qfmda.git # 关联本地代码库和远程代码库

git status # 查看仓库当前的状态，显示有变更的文件。
git log # 查看历史提交记录

git archive --format tar.gz --output "../archive/qfmda.year.mouth.tar.gz" master # 打包当前版本到 "../archive/qfmda.year.mouth.tar.gz"

git config -l # 查看当前git的配置
```



参考：

git: https://www.runoob.com/git/git-tutorial.html

Html: https://www.w3school.com.cn/html/index.asp