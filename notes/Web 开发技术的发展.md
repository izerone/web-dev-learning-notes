> Web 开发技术一直在不断发展，各种新的技术层出不穷。但是技术发展的本质是不变的，就是为了不断**提高生产效率**、**创造更好的产品和服务**和**解决更多更难的问题**。

# 一、静态页面时代

![静态页面时代](http://image-tter.qiniudn.com/blog/180829/3ccm94dj5d.jpg?imageslim)

- 缺点
    - 只能显示静态内容

# 二、动态页面

## 前后端不分

### 1.CGI 时代

![CGI Web](http://image-tter.qiniudn.com/blog/180829/BkJcbiImII.jpg?imageslim)

- CGI ( Common Gateway Interface ): 
    - 一种重要的互联网技术，可以让一个客户端，从网页浏览器向执行在网络服务器上的程序请求数据。CGI描述了服务器和请求处理程序之间传输数据的 **一种标准** 。( 摘自 [维基百科-通用网关接口](https://www.wikiwand.com/zh-sg/%E9%80%9A%E7%94%A8%E7%BD%91%E5%85%B3%E6%8E%A5%E5%8F%A3))
    - 可以用任何脚本语言或者是完全独立编程语言实现，Perl 使用的最广泛
- 缺点
    - 伸缩性差，每个请求分配一个新的进程
    - 不安全，直接访问文件系统或者环境变量

### 2.Servlet , JSP , ASP , PHP 等技术出现

![JSP Web](http://image-tter.qiniudn.com/blog/180829/mACI95Diab.jpg?imageslim)

- 缺点
    - 可维护性不好，UI 和业务逻辑高耦合
    - 前后端开发强关联，不利于提高开发效率

## 后端 MVC

![后端 MVC Web](http://image-tter.qiniudn.com/blog/180829/6A7Dg382HE.jpg?imageslim)

![MVC 软件架构](http://image-tter.qiniudn.com/blog/180829/Hcj5CcdakI.jpg?imageslim)
- **MVC**
    - MVC模式（Model–view–controller）是软件工程中的一种软件架构模式，把软件系统分为三个基本部分：模型（Model）、视图（View）和控制器（Controller）。( 摘自 [维基百科-MVC](https://www.wikiwand.com/zh-sg/MVC) )
        - **模型（Model）**  用于封装与应用程序的业务逻辑相关的数据以及对数据的处理方法。“ Model ”有对数据直接访问的权力，“Model”不依赖“View”和“Controller”，Model 不关心它会被如何显示或是如何被操作。但是 Model 中数据的变化一般会通过一种刷新机制被公布。为了实现这种机制，那些用于监视此 Model 的 View 必须事先在此 Model 上注册，从而，View 可以了解在数据 Model 上发生的改变。
        - **视图（View）** 能够实现数据有目的的显示。在 View 中一般没有程序上的逻辑。为了实现 View 上的刷新功能，View 需要访问它监视的数据模型（Model），因此应该事先在被它监视的数据那里注册。
        - **控制器（Controller）** 起到不同层面间的组织作用，用于控制应用程序的流程。它处理事件并作出响应。“事件”包括用户的行为和数据 Model 上的改变。

- 缺点
    - 业务逻辑并没有完全严格区分，JSP 中存在业务代码
    - 前端开发者需要了解后端语言

## 前后端分离

### 1. Ajax

![Ajax Web](http://image-tter.qiniudn.com/blog/180829/414FK2EKG6.jpg?imageslim)

### 2. JSON

![Ajax JSON Web](http://image-tter.qiniudn.com/blog/180829/A973blDhlE.jpg?imageslim)

### 3. 前端 MVC 

![Ajax JSON MVC Web](http://image-tter.qiniudn.com/blog/180829/69iJa1E97I.jpg?imageslim)

- 前后端分离的缺点
    - 不利于 SEO
    - 性能差，js 渲染页面时间长

### 4. Node.js

![Nodejs Server Web](http://image-tter.qiniudn.com/blog/180829/d13J8G1J5g.jpg?imageslim)

- 前端 UI layer 处理浏览器层的展现逻辑。通过 CSS 渲染样式，通过 JavaScript 添加交互功能，HTML 的生成也可以放在这层，具体看应用场景。
- Nodejs  UI layer 处理路由、模板、数据获取、cookie 等。通过路由，前端终于可以自主把控 URL。

# 三、相关技术知识点
## 基础知识
- HTML
- CSS
- JavaScript
- http 协议
- Linux 服务器常用命令
## 前端
- CSS 框架
    - Bootstrap
- 前端 MVC 框架
    - Vue
    - React
    - AngularJS
- Nodejs
## 后端 ( 以 Java 为主)
- Web 服务器
    - Apache HTTP
    - Nginx
- Web 应用服务器
    - Tomcat
    - Weblogic
    - WebSphere
- Servlet/JSP
- 后端 MVC 
    - SSH
    - SSM
    - SpringMVC
    - SpringBoot
    - SpringCloud
- 数据库
    - MySQL
    - Oracle
**参考链接:**
1. [Web开发的发展史](http://blog.jobbole.com/45169/)
2. [Web开发技术的演变](https://blog.csdn.net/juzipchy/article/details/76749311)
3. [Web开发技术的演变](http://blog.jobbole.com/45170/)

> 梳理技术的演进过程，是为了更全面的了解技术的变化，和对自己知识体系的查漏补缺，该文会不定期更新，同时欢迎大家一起讨论。