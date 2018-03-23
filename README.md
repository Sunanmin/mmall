**mmall project**
1.初始化项目:
http://blog.csdn.net/maomengmeng/article/details/52043928/
idea创建新的maven项目,项目构建成功后,可以通过File -->project Structure进行项目结构配置
Modules可以配置包路径,编译输出路径,jar依赖路径
Facets配置web 路径

tomcat服务器配置

2.git初始化
File-->settings-->Tools-->Terminal配置git终端命令
touch README.md           //创建README.md文件
touch .gitignore          //创建gitignore文件
git init                  //git仓库初始化
git status                //查看状态
git add .                 //添加到缓冲区
git status       
git commit -m "first commit init project"    //提交到代码仓库
git remote add origin https://github.com/Sunanmin/mmall.git   //与远程仓库进行关联
git branch                //查看分支
git push -u origin master //推送本地仓库到远程 
(username and password)
git branch      
git branch -r             //查看远程分支
git checkout -b v1.0      //创建新的分支 v1.0
git branch 
git push origin HEAD -u   //推送v1.0到远程上

3.pom.xml依赖配置及项目结构初始化
添加相关的依赖jar包 创建相关的包结构

4.mybatis generator自动生成代码
<plugin>
        <groupId>org.mybatis.generator</groupId>
</plugin>
pom.xml文件要有上面的插件引入,然后在resource目录下导入generatorConfig.xml文件
对generatorConfig.xml文件进行相关的配置改变,并在resource生成必要的datasource.properties文件
最后点击右侧MavenProject-->Plugin-->mybatis-generator:generate自动生成代码
时间戳优化:
   dao层对应的mapper中 insert和update语句字段 create_time和update_time改为now()

5.spring官方demo及配置
git:spring-petclinic   spring-greenhouse


