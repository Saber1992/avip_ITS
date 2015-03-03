# avip_ITS
List of ITS paper 


切到目标文件夹目录下，拉取远程文件，执行
```sh
git clone https://github.com/imerse/avip_ITS.git
```
每次要自己要编辑list文件之前都执行 
```sh
git pull —-rebase origin master
```
如果提示有confilct，需要先打开文件，会有三行类似 

> "=================HEAD"<br/>
> "==================="<br/>
> "===================[本次的提交编号]"


此时表示在你当前编辑的时候，别人同时编辑并push了，只需要简单Check一下上面三行之间的[文章]内容有没有重复，没有的话就直接删掉这三行，然后继续执行下面的命令；有重复表示你们同时找了相同的文章，嗯，私下解决删掉谁的，^_^。

编辑完成之后   
```sh
git add .  //将所有的更改增至索引   
git commit -am “message”   //message为本次改动的一个tag，可随意   
```
push到远程的分支
```sh
git push origin local_branch:master  //local_branch通常为master，如果没有特别设置过，直接用master就可以 
```
Done.