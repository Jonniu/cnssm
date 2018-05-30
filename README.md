# torchbearer 
 基于SSM框架的管理系统，支持操作权限和数据权限，后端采用Spring、SpringMVC、Mybatis、Shiro，前端采用adminLTE、vue.js、bootstrap-table、tree-grid、layer，对前后端进行封装，可快速完成CRUD的开发，基于项目结构通过代码生成器可生成前端后台部分代码，更加方便地进行二次开发。项目采用Maven分模块构建，方便扩展自定义模块。
 个人模仿（http://dp-dev.mydoc.io/）
### 技术方案
- 核心框架：Spring
- WEB框架：SpringMVC
- ORM框架：Mybatis
- 缓存框架：Ehcache、Redis
- 会话管理：Spring-session
- 安全框架：Shiro
- 模板框架：thymeleaf【视图解析器】、velocity【代码生成器】（支持freemarker、jsp等其他自定义视图）
- 主页框架：adminLTE(Bootstrap)
- JS框架：vue.js
- 表格插件：bootstrap-table
- 树形表格：tree-grid(基于bootstrap扩展)
- 树形插件：ztree
- 弹窗组件：layer
- 表单校验：validator
- 日期组件：laydate
- 后端校验：fluent-validator
- 接口管理：swagger-ui
### 项目结构
cnssm-base 基础模块
cnssm-web  前端界面
cnssm-shiro 权限模块
cnssm-common 公共通用模块
cnssm-orm  数据持久模块
cnssm-generator  代码生成模块
### 项目介绍
- 前后端开发封装，快速实现CRUD开发
- 支持通过velocity模板生成部分代码，可直接生成到项目路径，无须二次部署（见文档）
- 基于角色的权限管理，细分到按钮权限和数据权限
- 基于Maven模块化开发，可快速扩展个性化业务模块
- 支持单页iframe嵌套和多页tab标签框架
- 支持分布式session管理，能够集群部署
- 支持数据库读写分离，动态切换数据源
- 支持Mybatis-Ehcache二级缓存
### 命名规范（参考阿里巴巴Java开发手册）
-  获取单个对象的方法用 get 做前缀
-  获取多个对象的方法用 list 做前缀
-  获取统计值的方法用 count 做前缀
-  插入的方法用 save(推荐) 或 insert 做前缀
-  删除的方法用 remove(推荐) 或 delete 做前缀
-  修改的方法用 update 做前缀
### 应用分层（参考阿里巴巴Java开发手册）
![image](http://oss.chenlintech.com/common/0.png)