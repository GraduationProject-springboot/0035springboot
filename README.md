# [首页查询更多项目](https://github.com/GraduationProject-springboot) 包安装运行


# 0035springboot海滨体育馆管理系统的设计与实现

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV16ia6epENY?p=36)


# 课题背景
当今时代是飞速发展的信息时代。在各行各业中离不开信息处理，这正是计算机被广泛应用于信息管理系统的环境。计算机的最大好处在于利用它能够进行信息管理。使用计算机进行信息控制，不仅提高了工作效率，而且大大的提高了其安全性。尤其对于复杂的信息管理，计算机能够充分发挥它的优越性。

据调查，传统的海滨体育馆管理面对大量学生信息、器材信息、器材归还信息、进入/离开登记信息以及活动预约信息等，信息的及时更新等弊端凸显，传统的海滨体育馆管理过度的依靠人力资源的登记，对于庞大的信息量，显然只依靠人力，很难准确的处理好大量的数据，传统的管理模式不仅效率低，出错率高，对于海滨体育馆管理带来了诸多不便，因此，传统的海滨体育馆管理模式已经远远无法满足管理需求，我们急需对海滨体育馆管理体系进行变革，开发基于计算机平台的海滨体育馆管理系统。现代化的利用计算机来进行海滨体育馆管理很大程序上可以提高效率，人力方面也大大的节省，界面简单易操作，只要会计算机就可以快速的进行海滨体育馆相关信息的管理。对经济方面也是很大的节省，其优点是显而易见的。

基于Spring Boot的海滨体育馆管理系统实现了海滨体育馆管理的自主化、智能化，达到提高管理效率和质量，节省人力资源。
1. ## 设计原则
在开始开发项目之前，必须要先考虑项目的实用性、科学性，以及该项目是否能够真正让用户受益并尽可能的发挥项目的作用。因此，在开发前，通过以下几条原则对项目进行判断：

（1）可行性原则。项目需要保证经济可行性和技术可行性，这包括了项目在浏览端、服务端等方面上的经济和技术上是可以达成的。

（2）适应性原则。项目要保证可维护性和可扩展性，这是每个非短期项目都需要考虑的，并且不论是维护还是扩展，都必须要建立在适应用户的正常需求的基础上。

（3）安全性及保密性原则。要充分保证用户信息的安全性和保密性，不能因为开发上的疏忽，导致用户的信息泄露。

（4）系统工程原则。为了确保项目的整体性，在项目调查、项目分析、项目设计、项目开发的过程中，都需遵从项目工程的方法和步骤逐步进行。

（5）统一规划、分期实施、逐步完善原则。项目开发的过程中，要按照规划、分期实施，特别是要注意在项目开发过程中要有条理，从点到面，一步步完善，不要贪图进度，要循环渐进的对项目进行开发。
1. ## 论文结构安排
对本文所涉及的相关技术进行学习，系统的分析是一个很重要的环节，更好的进行程序的设计，必须进行前期的深入调查，对系统进行全面的功能设计，和详细的解析。课题最主要的工作是通过Java+MYSQL建立一个完善的海滨体育馆管理系统，系统最主要的模块是海滨体育馆相关信息的管理。本文主要分为六大部分：

第一部分绪论介绍了本文的研究背景和设计原则，为系统的开发奠定基础。

第二部分主要是是介绍了基于Spring Boot的海滨体育馆管理系统所采用的技术，开发环境。

第三部分对基于Spring Boot的海滨体育馆管理系统进行分析，包括可行性分析，系统功能需求，系统流程分析等。

第四部分进行系统的设计，这一部分是系统主要的数据库部分，介绍功能结构和数据库的设计等。

第五部分总结了系统的界面和实现过程进行分析。

第六部分主要是对系统测试进行阐述，对测试遇到的问题进行说明。

1. # 系统关键技术
   1. ## JAVA技术
Java是一种非常常用的编程语言，在全球编程语言排行版上总是前三。在方兴未艾的计算机技术发展历程中，Java的身影无处不在，并且拥有旺盛的生命力。Java的跨平台能力十分强大，只需一次编译，任何地方都可以运行。除此之外，它还拥有简单的语法和实用的类库，让编程人员可以尽可能将精力集中在问题的求解上，并且许多开源项目和科研成果都是采用它实现的。

在1995年这一年的5月份，著名的Sun Microsystems公司在程序开发设计上面郑重推出一种面向对象开发的程序设计语言——Java，最开始的时候Java是由詹姆斯.高斯林这位伟大的JAVA之父来进行主导，但是在后来由于各种原因，让甲骨文公司这个针对商业程序创建了oracle大型数据库的公司收购了Java[1]。Java的平台总共算下来有3个，分别为javaME和javaSE以及javaEE这3个java平台。下面将对其进行分别介绍。

（1）在电脑桌面程序的开发上面需要选择JavaME，这个用得也比较多。

（2）企业也会根据工作以及业务需要开发各种软件，那么就会选用JavcEE这个支持企业版软件的开发的Java平台，JavcEE主攻运用在企业领域上面的web应用，JavcEE也在javaSE的基础上获得了比如jsp技术 ，Servlet技术等程序开发技术的支持。

（3）现在生活中手机的普及化，也使得手机端这样的移动设备的软件的兴起，JavaME这个迷你版java平台就能运用于移动端的软件开发操作。
1. ## B/S结构
B/S（浏览器/服务器）结构是目前主流的网络化的结构模式，它能够把系统核心功能集中在服务器上面，可以帮助系统开发人员简化操作，便于维护和使用。

在早期的程序开发中，使用得最多的莫过于C/S架构了，现在的生活中软件在生活的各个方面落地，使用了C/S架构开发出来的软件也是不在少数的，比如企业日常办公使用到的微软的OFFICE软件，我国自己研发的文档处理软件WPS，还有娱乐软件腾讯的QQ，腾讯的微信，以及电脑上安装的杀毒软件金山杀毒软件，瑞金杀毒软件等都是C/S架构。但是在Internet网络盛行之后，鉴于大家对数据信息共享的需求，在原来的C/S架构上进行了升级改进之后，有了现在的主流架构B/S架构，B/S架构就是在C/S架构上多了一个浏览器，让原来的直接访问服务器的方式，变成了通过浏览器去访问服务器。充分运用到了当下不断成熟的浏览器技术。也让软件的开发成本以及维护成本降低了。可以说B/S这种新型的架构模式让软件的开发变得便利化。

B/S架构不需要在任何客户端来进行程序的部署，使用这样的程序结构来使用开发好的系统是利用浏览器来使用的，就是把开发好的程序配置到一台远程服务器上，在任何可以访问这台服务器的客户端电脑上都可以对程序进行操作和使用，这样的方式给使用者带来了极大的便捷。这样的结构提高了程序的运行效率，打破了地域的限制，降低了程序的使用成本。
1. ## MYSQL数据库
所谓数据库，实际上就是一个容器，按照数据结构来组织、存储和管理。数据库的作用就是为大量的信息进行管理并提供高效的解决方案。

MySQL是典型的关系数据库系统，拥有开源免费、稳定、高效等特点，一直是中小型web项目的最佳数据库选择。MySQL作为当今IT领域使用人数最多的开源关系型数据库软件之一，在2018年的数据库使用率排名中位居第二，仅次于目前为止最成功的商业版数据库Orcle[13]。MySQL最大的优势之一就是无偿使用，这也是它成功的关键。

MySQL支持标准化数据库查询语言SQL。MySQL是一款非常适合个人开发者或小型组织开发团体的数据库管理系统，因为它是开源并且免费的，体积小、速度快、成本低以及其最重要的一点开放源码，深受程序设计人员的喜爱，这也让它成为了许许多多中小型开发网站数据库的首选，同时提供了多种开发的连接API。MySQL将数据的存放按照记录之间的关系存放到了不同的表中，减少了数据的冗余并且提高了开发的工作效率。MySQL支持开发中需要用的大型数据库，并能处理数以万计的记录。因为MySQL是开源的软件，所以在项目的预算中的时候不用花费额外的资金，大大降低了开发的总体成本，这也是MySQL数据库在中小型企业和独立的开发者中广泛流行的原因[5]。
1. ## Spring Boot框架
Spring Boot是一个简化程序设置的拥有开箱即用的框架，它主要的优点是根据程序员不同的设置而生成不同的代码配置文件，这样开发人员就不用每个项目都配置相同的文件，从而减低了开发人员对于传统配置文件的时间，提高了开发效率。它内嵌Tomcat服务器，简化了Maven的配置，自动配置Spring，通过这样的框架，开发人员就不用头疼各种配置文件，可以减少时间，同时提高了代码的整体性，使开发人员工作效率大大提高。

1. # 系统分析
   1. ## 可行性分析
在进行可行性分析时，我们通常根据软件工程里方法，通过四个方面来进行分析，分别是技术、经济、运行和法律可行性。因此，在基于对目标系统的基本调查和研究后，对提出的基本方案进行可行性分析
1. ### 技术可行性
技术可行性一是考虑客观的技术可行性，二是考虑实际的技术可行性。从客观上、简单地说，现已经出现了类似的系统，因此客观上的可行性是满足的。从现有的实际情况上来看，该系统使用的是JAVA开发语言、MYSQL都是容易获得的，同时计算机的硬件性能也满足开发软件的需求；且在本科课程中都有进行相关软件的学习和开发。综上所述，该系统具有技术可行性。
1. ### 经济可行性
开发该系统时，优先考虑了使用网页来完成该系统。从已有的Web网页开发的案例、资料中，可知Web所需要的软硬件简单，切开发成本低。且从引进该系统后的预想表现将会比传统方式优异，其具有高效、低成本的特点。可以大量节省管理的人力、物力，具有一定经济效益和社会效益。综上所述，该系统具有高经济可行性
1. ### 运行可行性
运行可行性是对组织结构的影响，现有人员和机构和环境对系统的适应性及人员培训补充计划的可行性。以目前信息技术的普及程度之广、相关工作的操作人员的水平之高，是足以胜任的。综上所述，该系统具有高运行可行性。
1. ### 法律可行性
（1）所使用的技术或者资料（书籍、文献、软件）合乎中国法律。

（2）所开发过程不涉合同、侵权、责任和各种法律相抵的问题。

（3）所完成系统不存在侵犯版权问题。

（4）完全符合中国的《中华人民共和国著作权法》和《计算机软件保护条例》。

综上所述，该系统具有高法律可行性。

通过分析论证，该系统总体上是具有高可行性的。
1. ## 系统性能分析
达到如以下的性能需求指标，可以保证系统的安全性、可靠性、稳定性，需要：

（1）系统响应的精确性和实时性

这是本系统必要的性能。考虑到未来系统可能承受的工作量，需要能够承担得起企业级的信息处理需求。实时性是该系统的生命线，因此需采用软实时系统来进行保证。

（2）系统的开放性和系统的可扩充性

本系统是一个较为初期的一个雏形，以后势必会根据的海滨体育馆管理需求的扩大或转变。这就要求本系统需要提供足够的开放型和可扩充性，只要符合本系统的设计准则都可以将新的模块加入。通过这样的升级、维护来完成本系统后期的生命周期。

（3）系统的易用性和易维护性

开发的系统要求不论是熟悉或不熟悉计算机的人员都可以对系统进行有效的人机交互。因此提供给用户一个友好、漂亮的图形接口是非常重要的。这可以通过发一些纸质和实际的界面模型问卷调查来获得最佳的效果。此外，也考虑到维护本系统的操作人员，有效的手段的数据备份、管理和错误检测、恢复需要被提供给相关的人员。

（4）系统的响应速度

要求系统在任何情况下的平均响应速度达到秒级，具有软实时性。一是为了保证了系统的工作效率，二为了防止系统因同一时间段大量的用户登录系统而造成错误、瘫痪。
1. ## 系统功能分析
本基于Spring Boot的海滨体育馆管理系统主要实现了管理员功能模块和学生功能模块两大部分，这两大功能模块分别实现的功能如下：

（1）管理员功能模块

管理员登录后可对系统进行全面管理操作，包括个人中心、学生管理、器材管理、器材借出管理、器材归还管理、器材分类管理、校队签到管理、进入登记管理、离开登记管理、活动预约管理、灯光保修管理、体育论坛以及系统管理。管理员用例图如图3-1所示。

![](/md/blog.001.png)

图3-1 管理员用例图

（2）学生功能模块

学生在系统前台可查看系统信息，包括首页、器材、体育论坛以及体育资讯等，没有账号的学生可进行注册操作，注册登录后主要功能模块包括个人中心、器材管理、器材借出管理、器材归还管理、校队签到管理、进入登记管理、离开登记管理、活动预约管理，学生用例图如图3-2所示。

![](/md/blog.002.png)

图3-2  学生用例图
1. ## 系统流程分析
   1. ### 注册登录流程
没有账号的学生可进行注册操作，注册后可进行登录，注册登录流程如图3-3所示。

![](/md/blog.003.png)

图3-3 注册登录流程图
1. ### 添加信息流程
用户在添加信息时，系统编号自动生成生成，用户需要输入信息，系统会其进行验证，验证通过则添加成功，反之添加失败，添加信息流程如图3-4所示。

![](/md/blog.004.png)

图3-4 添加信息流程图
1. ### 删除信息流程
用户可选择需要删除的数据进行删除信息操作，删除信息流程如图3-5所示。

![](/md/blog.005.png)

图3-5 删除信息流程图

1. # 系统设计
   1. ## 系统概要设计
本海滨体育馆管理系统并没有使用C/S结构，而是基于网络浏览器的方式去访问服务器，进而获取需要的数据信息，这种依靠浏览器进行数据访问的模式就是现在用得比较广泛的适用于广域网并且没有网速限制要求的B/S结构，图4-1就是开发出来的程序工作原理图。

![](/md/blog.006.png)

图4-1 系统工作原理图
1. ## 系统结构设计
在系统结构设计过程中，首先，整个系统分成几个小的模块，小的问题，然后，进一步细分模块，添加细节。本基于Spring Boot的海滨体育馆管理系统结构图如图4-2所示。

![](/md/blog.007.png)

图4-2 系统结构图
1. ## 系统顺序图设计
（1）登录模块顺序图

登录模块主要满足了管理员和学生的权限登录，登录模块顺序图如图4-3所示。

![](/md/blog.008.png)

图4-3 登录模块顺序图

（2）添加信息模块顺序图

管理员和学生登录后均可进行添加信息操作，添加信息模块顺序图如图4-4所示。

![](/md/blog.009.png)

图4-4 添加信息模块顺序图
1. ## 数据库设计
   1. ### 数据库E-R图设计
E-R图是一种描述显示数据类型间的关系的数据描述方法，E-R图可以完整地映射出现实模型的关系。E-R图中的三个最为重要的元素就是实体、属性、关系。E-R图即由这三点组成。

实体：E-R图中数据的实体，用矩形表示上面为实体名，下面为实体属性，实体包含主外键等关系。

属性：E-R图中的属性，是指实体的属性，实体由多条属性所构成，属性拥有自己的数据类型，数据大小。属性的优劣决定了E-R图中实体的健全性、完整性。

关系：E-R图中的关系是指实体之间的关系，用菱形来表示实体间的关系，这些菱形关系的联系上有着一对多或多对多的数据联系，这些构成了E-R图的关系，E-R图的关系紧密连接了实体，使实体间的关联性更加的显著、易懂。本基于Spring Boot的海滨体育馆管理系统的E-R图如下所示：

（1）体育论坛信息实体E-R图如图4-5所示：

![](/md/blog.010.png)

图4-4  体育论坛信息实体E-R图

（2）活动预约信息实体E-R图如图4-5所示：

![](/md/blog.011.png)

图4-5  活动预约实体E-R图

（3）器材信息实体E-R图如图4-6所示：

![](/md/blog.012.png)

图4-6  器材信息实体E-R图

（4）管理员信息实体E-R图如图4-7所示：

![](/md/blog.013.png)

图4-7  管理员实体E-R图

（5）学生信息实体E-R图如图4-8所示：

![](/md/blog.014.png)

图4-8  学生实体E-R图
1. ### 数据库表设计
基于Spring Boot的海滨体育馆管理系统采用MYSQL数据库系统进行系统数据的储存，下面介绍数据库中的各个表的详细信息。

表4-1  forum体育论坛信息表

|字段名称|字段意义|字段类型|字段长度|是否主键|能否为空|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|编号|bigint|20|是|否|
|addtime|创建时间|timestamp||否|是|
|title|帖子标题|varchar|200|否|是|
|`content|帖子内容|longtext||否|是|
|`parentid|父节点编号|bigint|20|否|是|
|userid|用户编号|bigint|20|否|是|
|username|用户名|varchar|200|否|是|
|isdone|状态|varchar|200|否|是|

表4-2  huodongyuyue活动预约信息表

|字段名称|字段意义|字段类型|字段长度|是否主键|能否为空|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|编号|bigint|20|是|否|
|addtime|创建时间|timestamp||否|是|
|yuyuebumen|预约部门|varchar|200|否|是|
|yuyuechangdi|预约场地|varchar|200|否|是|
|huodongneirong`|活动内容|longtext||否|是|
|yuyuexiangqing|预约详情|longtext||否|是|
|yuyueshijianduan|预约时间|varchar|200|否|是|
|xuehao|学号|varchar|200|否|是|
|xingming|姓名|varchar|200|否|是|
|nianjibanji|年级班级|varchar|200|否|是|
|tijiaoshijian|提交时间|datetime||否|是|
|fengmiantu|封面图|varchar|200|否|是|
|`sfsh|是否审核|varchar|200|否|是|
|shhf|审核回复|longtext||否|是|

表4-3  qicai器材信息表

|字段名称|字段意义|字段类型|字段长度|是否主键|能否为空|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|编号|bigint|20|是|否|
|addtime|创建时间|timestamp||否|是|
|qicaibianhao|器材编号|varchar|200|否|是|
|qicaimingcheng|器材名称|varchar|200|否|是|
|qicaifenlei|器材分类|varchar|200|否|是|
|qicaizhuyishixiang`|器材注意事项|longtext||否|是|
|qicaishuoming|器材说明|longtext||否|是|
|qicaitupian|器材图片|varchar|200|否|是|

表4-4  users管理员信息表

|字段名称|字段意义|字段类型|字段长度|是否主键|能否为空|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|编号|bigint|20|是|否|
|username`|用户名|varchar|200|否|是|
|password|密码|varchar|200|否|是|
|role|角色|varchar|200|否|是|
|addtime|新增时间|timestamp||否|是|

表4-5  xuesheng学生信息表

|字段名称|字段意义|字段类型|字段长度|是否主键|能否为空|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|编号|bigint|20|是|否|
|addtime|创建时间|timestamp||否|是|
|xuehao|学号|varchar|200|否|是|
|mima|密码|varchar|200|否|是|
|nianjibanji|年级班级|varchar|200|否|是|
|xingming|姓名|varchar|200|否|是|
|xingbie|性别|varchar|200|否|是|
|shoujihaoma`|手机号码|varchar|200|否|是|
|youxiang|邮箱|varchar|200|否|是|
|zhaopian|照片|varchar|200|否|是|
|beizhu`|备注|longtext||否|是|



1. # 系统的实现
   1. ## 登录模块的实现
管理员和学生在登录界面输入用户名、密码，选择类型进行登录操作，系统登录界面展示如图5-1所示。

![](/md/blog.015.png)

图5-1系统登录界面图
1. ## 注册模块的实现
没有账号的学生用户可进行注册操作，学生注册界面如图5-2所示。

![](/md/blog.016.png)

图5-2  学生注册界面
1. ## 学生管理模块的实现
管理员可添加、修改和删除学生信息，学生管理界面如图5-3所示。

![](/md/blog.017.png)

图5-3 学生管理界面
1. ## 系统主界面模块的实现
学生可进入系统前台查看系统信息，包括首页、器材以及体育论坛等，系统主界面如图5-4所示。

![](/md/blog.018.png)

图5-4 系统主界面
1. ## 器材管理模块的实现
管理员可以添加、修改和删除器材信息，学生可查看器材信息，器材管理界面展示如图5-4所示。

![](/md/blog.019.png)

图5-5 器材管理界面
1. ## 器材借出管理模块的实现
学生可添加器材借出信息，管理员可查看管理所有器材借出信息，并可对其进行修改和删除操作，同时也可添加器材借出信息，器材借出管理界面如图5-6所示，添加器材借出界面展示如图5-7所示。

![](/md/blog.020.png)

图5-6 器材借出管理界面

![](/md/blog.021.png)

图5-7 添加器材借出界面
1. ## 活动预约管理模块的实现
学生可添加活动预约信息，管理员可查看活动预约信息，并可对其进行审核、修改和删除操作，活动预约管理界面如图5-8所示，添加活动预约界面展示如图5-9所示。

![](/md/blog.022.png)

图5-8 活动预约管理界面

![](/md/blog.023.png)

图5-9 添加活动预约界面
1. #










