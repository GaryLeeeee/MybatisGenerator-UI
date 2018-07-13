# MybatisGenerator-UI

[![Join the chat at https://gitter.im/MybatisGenerator-UI/Lobby](https://badges.gitter.im/MybatisGenerator-UI/Lobby.svg)](https://gitter.im/MybatisGenerator-UI/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Travis](https://img.shields.io/travis/rust-lang/rust.svg)]()[![apm](https://img.shields.io/apm/l/vim-mode.svg)]()

Mybatis Generator UI is based on [Mybatis Gennerator](http://www.mybatis.org/generator/). It provides a web tool to generate code.


#### Screenshot

![](http://ww1.sinaimg.cn/large/006tNc79gy1ffne57i7enj31kw0zk0z4.jpg)

-------


#### Quick Start

* Clone the project if you haven't yet.

```
git clone https://github.com/lishuo9527/MybatisGenerator-UI.git
```

* Build the project with the code


```
cd MybatisGenerator-UI
mvn clean package -Dmaven.test.skip
```

*  Change default server port from application.properties file if you want.

```
### Default server port #########
server.port=8888
```

* Run it from the command line with a command like this:

```
cd target/
nohup java -server -Xms128m -Xmx128m -jar MybatisGenerator-1.0.0-SNAPSHOT.jar  >out.log 2>&1 &
```

* you can also run it in Eclipes or IntelliJ IDEA. Just find class `me.lishuo.MybatisGeneratorApplication` and run it.

*  Access server  as `http://localhost:8888`


#### TODO
* Support more databases( Now only support MySQL)
* Optimize code
* ~~Add system configuration~~(Done)


#### License
Mybatis Generator UI is released under the [MIT License](https://github.com/lishuo9527/MybatisGenerator-UI/blob/master/LICENSE).


#### GaryLee做的小笔记
* 端口默认为6666,可在application.properties查看及修改
* 操作步骤:
```
1.启动MybatisGeneratorApplication
2.打开http://localhost:6666/
3.输入各项参数(包名为文件夹名,可用.分隔子文件夹,如com.garylee.demo.domain)
4.模型名称为实体类名(domain)
5.生成,保存压缩文件(保存实体类和dao文件,默认名为mbg)
```
