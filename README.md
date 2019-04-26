自动构建工具使用

安装包命令： go get github.com/whr-helen/go-struct-auto



注释：参数信息

-d dbname 改为自己数据库的名称  （必填）

-path ./models 改为存放路径   (可选默认为./models )

-t  account,user 改为要生成的表名称、可多个  (可选默认全部生成)



一、生成数据库所有表 结构体：

① 推荐使用方法(支持 linux or mac)

生成命令： ./bin/automatic -d dbname  -path ./models


② 修改生成工具代码(支持 linux or mac or windows)如果生成出来的结构不是我们所需要的可以修改 automatic.go 文件

命令： go run automatic.go -d dbname -path ./models

二、生成单个多个表 结构体：

命令(支持 linux or mac)： ./bin/automatic -d dbname -t account,user


命令(支持 linux or mac or windows)： go run automatic.go -d dbname -t account,user