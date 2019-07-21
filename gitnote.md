# git配置
- [.gitignore](#1)


1 .gitignore


	使用场合：
	忽略操作系统自动生成的文件，比如：缩略图，等；
	忽略编译生成的中间文件、可执行文件等，比如： C 语言编译产生的 .obj 文件和 .exe 文件；
	忽略你自己的带有敏感信息的配置文件，比如：存放口令的配置文件；
	tmp/ 临时目录；
	log/ 日志目录
 

     
- vim .gitignore #编辑gitignore文件，加入要忽略的文件  
- git add -f file #强制添加被忽略的文件
- git check-ignore -v file #查看file在.gitignore中的位置

- [我的testignore库](https://github.com/zhenxuanzhang/testignore)
- [github官方gitignore库](https://github.com/github/gitignore)


## 
