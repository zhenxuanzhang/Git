# git配置


---
- [.gitignore](#1gitignore)

---
## 1.gitignore


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

## 2.换行符

	# CR: carriage return 回车，光标到首行， ‘\r’ = return
	# LF: line feed 换行，光标下移一行，’\n’ = newline
	# linux: 换行 \n
	# windows: 换行 \r\n
	# MAC OS: 换行 \r

	# 提交时转换为LF，检出时转换为CRLF，默认设置不用修改，Git 是 linux 配置
	git config –-global core.autocrlf true
	# 允许提交包含混合换行符的文件
	git config –-global core.safecrlf false

## 3.别名

	# 以图形的方式打印 Git 提交日志
	git log –pretty=format:’%h %ad | %s%d’ –graph –date=short

	# 设置别名
	git config –-global alias.ci commit
	
## 4.凭证
	# 存储凭证
	git config –-global credential.helper wincred

