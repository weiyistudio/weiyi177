# weiyi177
基于SSM架构的个人博客系统的实现

# 基于SSM架构的个人博客系统的实现

#### 介绍
随着网络越开越发达，越来越多的网络用户希望能够在网络平台上更多地展现自己的个性，更方便地与人互动交流，在传统的WEB1.0时代，无论是论坛、社区还是个人网站，都试图在这些方面进行努力，随着WEB2.0时代的到来，一个新的概念出现--博客。它已经成为写网络日志必不可少的一种工具，也是一种简单有效的提供网络用户之间进行在线交流的网络平台，通过其可以结交更多的朋友，表达更多的想法，它随时可以发布日志，方便快捷。个人博客的发展，也已经成为广告商业务拓展的重要领域。
本论文主要介绍了系统的分析，设计和开发的全部过程。运用数据流图、E-R图、程序流程图等对系统的设计过程进行详细的说明，全文共分为项目概述、需求分析、系统设计、系统实现，系统测试几大部分。本系统的集成开发环境是IDEA，前端使用了JSP等技术，数据库管理运用了MySQL，Web服务器采用Tomcat，另外还采用SSM框架技术和B/S结构。
本系统经过测试，能够正常的运行，功能完善，性能较高，页面比较简洁。在不需要查看操作帮助的情况下也能轻松直观的操作。总的来说这个系统开发比较成功。














#### 项目说明
![输入图片说明](https://images.gitee.com/uploads/images/2021/0209/013200_3503fbda_8621591.png "屏幕截图.png")

便捷性：系统以便捷的信息访问为首要目标，以方便用户使用为核心原则，需要充分考虑实际操作的各项细节，本系统努力做到尽善尽美，最终通过用户的不断反馈将及时调整，力争做到方便用户操作。在不需要查看操作帮助的情况下也能轻松直观的操作，并对操作流程有清晰的理解。 
实用性：包括系统功能和系统信息呈现以使用为目标，不添加华而不实的部件与功能，既不丢失必要的信息，又能简单直观，以传达信息为核心，对文字记录提供较好的封装。另外通过系统能够及时了解更多的信息，体现系统的核心价值。
可靠性：由于多用户的访问，因此系统要具备可靠的性能处理要求，要求数据存取可靠安全，尽量避免丢失用户创建的资料或数据状态不一致现象。
可维护性：针对系统后期的功能调整或增删，应尽量减少维护的工作量。对系统中的资料操作也应该方便查阅与修改。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0209/013226_eb9efc44_8621591.png "屏幕截图.png")

（1）管理员信息表(admin)
管理员信息表主要用于保存系统管理员的信息，主要字段包括：管理员ID、登录账号、登录密码。表结构如表4.1所示。
 
表4.1管理员信息表
列名	数据类型	长度	允许空	是否主键	说明
id	int	10	否	是	管理员ID
username	varchar	12	否	否	登录账号
password	varchar	15	否	否	登录密码
（2）用户信息表(user)
用户信息表主要是记录了用户基本信息，表结构如表4.2所示。
表4.2 用户信息表
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	用户ID
username	varchar	50	否	否	用户名
password	varchar	50	否	否	密码
（3）博客文章表(report)
博客文章表主要是记录了文章的基本信息，表结构如表4.3所示。
表4.3博客文章表
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	ID
title	varchar	50	否	否	文章题目
content	varchar	50	否	否	文章摘要
summary	varchar	100	否	否	文章内容
category	varchar	50	否	否	分类ID
createTime	varchar	50	否	否	创建时间
top	int	4	否	否	优先级
 
（4）文章分类表(category)
文章分类表主要是文章分类的相关信息，其中ID是主键，表结构如表4.4所示。
表4.4文章分类表
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	ID
title	int	4	否	否	分类名称
createTime	varchar	50	否	否	创建时间
（5）常用链接表(like)
常用链接表主要是常用链接的相关信息，其中ID是主键，表结构如表4.5所示。
表4.5常用链接表
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	ID
name	varchar	40	否	否	链接名称
src	varchar	50	否	否	链接网址
createTime	varchar	50	否	否	创建时间
（6）文章评论表(comment)
文章评论表主要是文章评论的相关信息，其中ID是主键，表结构如表4.6所示。
表4.6文章评论表
列名	数据类型	长度	允许空	是否主键	说明
id	int	4	否	是	ID
User	varchar	20	否	否	用户名称
Content	varchar	50	否	否	评论内容
createTime	varchar	50	否	否	创建时间






#### 项目截图
![输入图片说明](https://images.gitee.com/uploads/images/2021/0209/013307_44d9cdeb_8621591.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/0209/013329_fa15fadf_8621591.png "屏幕截图.png")

[图片上传失败(image-5WKymaGh2RILaMnMoW4d)]



#### 求助热线


代码有任何问题可联系
联系Q：2762501186

                            
![输入图片说明](https://images.gitee.com/uploads/images/2020/1119/003728_cd598bb9_4865385.jpeg "微信.jpg")           

感谢Github！！  
觉得项目不错的给个Star谢谢大佬！！！
提供无偿review服务
