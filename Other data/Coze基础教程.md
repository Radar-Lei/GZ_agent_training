> 🔊 **版权说明：** 著作权归作者所有，侵权必究！

> **写在前面：** 本教程是我在使用扣子搭建应用过程中，对知识的系统化总结。每一个案例都是亲自反复测试，文字也是逐字逐句检查后通过键盘敲出来的，目的就是让大家在学习的过程中少走一些弯路。希望大家给个关注支持一下，谢谢！

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/img_qrcode-inys.png)

## 引言

## 1\. 什么是AI应用开发

首先明确一下**AI应用开发**的定义。广义来说：AI应用开发是指利用人工智能（Artificial Intelligence, AI）技术来设计、构建和维护软件应用程序的过程。

在我们教程里的**AI应用开发**指的是：**利用大语言模型(LLM) 应用开发平台快速搭建生产级的生成式 AI 应用。**

例如：如果你是文案编辑人员，你可以利用可以开发一款**文案写作**应用，提高自己的文案写作效率； 如果你是一名**股票玩家**，你可以开发一款股票分析应用，实时分析市场行情，为投资指点迷津。

而且相比代码开发方式，即使你是非技术人员，也能参与到 AI 应用的定义和数据运营过程中。

## 2\. 为什么要学习AI应用开发

通过学习AI应用开发，可以帮助你提高工作效率，减少重复性劳动。  
学习AI应用开发可以帮助开发者掌握最新的AI应用开发技能，保持竞争力。你可以通过开发自己的应用，解决公司的复杂的业务流程。如果你开发一款解决某些行业痛点的AI应用，也可以进行出售，赚取利润。  
目前AI技术正迅速改变众多行业，学习AI应用开发不仅仅是为了掌握一个特定的工具，更是为了理解和利用AI技术来推动个人和企业的发展。

## 3\. AI应用开发平台有哪些

大语言模型(LLM) 应用开发平台目前有很多，例如：扣子(Coze)、Dify、Fastgpt、Langchatchat、Flowise、Langflow、Bisheng等这些都是目前一些主流的开发平台。在本教程中，我们先来学习扣子(Coze)的应用开发。

## 1\. 什么是扣子

扣子是新一代 AI 应用开发平台。无论你是否有编程基础，都可以在扣子上快速搭建基于大模型的各类 Bot，并将 Bot 发布到各个社交平台、通讯软件或部署到网站等其他渠道。

## 2\. 扣子的功能与优势

**用户友好的界面**：Coze的操作界面设计合理，逻辑清晰，易于上手，符合用户的使用习惯。

**功能丰富**：平台提供了包括插件系统、记忆库、工作流等在内的多种功能，用户可以根据自己的需求灵活选择和配置这些功能。

**支持知识库和自定义插件**：用户不仅可以导入数据到知识库，还可以自定义插件来扩展机器人的能力，提高了系统的可定制性。

**多平台部署**：构建的机器人可以部署到微信、飞书等社交媒体平台以及企业内部应用程序，增加了系统的灵活性和适用性。

**无需编程基础**：Coze平台几乎不需要编程基础，模型、插件、知识库等核心技术都进行了封装，使得用户可以快速搭建Bot。

**免费使用**：至少在现阶段，Coze平台是完全免费的，为用户提供了易于使用的AI Bot开发环境。

**集成插件工具集**：Coze平台集成了超过种多样化的插件工具，覆盖了新闻阅读、旅行规划等多个领域，支持用户快速为机器人添加功能。

**增强聊天机器人能力**：Coze平台还提供了工作流、知识库等功能，以及长期记忆和定时任务等，增强了聊天机器人的能力和交互性。

**国际版与国内版**：Coze有国内版和国际版，国际版提供了更完善的GPT-4模型功能，而国内版可能存在一些限制。

## 3\. 注册和基本界面介绍

注册登录Coze平台的步骤比较简单，你可以直接访问Coze官网进行注册，使用邮箱或手机号完成账户信息的填写和验证。

::: tip 🌐 平台地址: [https://www.coze.cn/](https://www.coze1.cn/ "Coze平台地址")  
:::

登录成功后，你会看到Coze的基本界面。在界面的左上角，你可以点击"创建 Bot"按钮来创建一个新的Bot。  
![](https://www.bzfree.com/upload/images/coze/login.png)

创建机器人时，你需要输入Bot的基本信息，如名称、头像等。这些信息可以随意填写，主要用于标识你自己使用的机器人。

![](https://www.bzfree.com/upload/images/coze/coze2.png)

在机器人配置页面，界面主要分为三栏：

-   最左边是Bot提示词编写页面，可以在这里设定机器人的角色、技能和限制。

![](https://www.bzfree.com/upload/images/coze/coze3.png)

-   中间一栏是功能最丰富的地方，可以配置官方提供的插件、自定义工作流、引入知识库内容或创建数据库。

![](https://www.bzfree.com/upload/images/coze/coze4.png)

-   Coze平台提供了Bots、插件、工作流和知识库四个主要功能，这些功能都会在创建机器人的过程中用到。
-   在创建机器人的过程中，你还可以利用Coze提供的数据库功能，创建数据集合，定义字段，类似于传统数据库的表结构设计。
-   最右边是调试页面，在调试页面可以直接和机器人进行对话，查看返回结果是否符合预期。

![](https://www.bzfree.com/upload/images/coze/coze5.png)

-   当你完成所有相关设置后，可以点击右上角的发布按钮，将机器人发布到Coze的应用商店。

![](https://www.bzfree.com/upload/images/coze/coze6.png)

## 第二章：快速开始

> 🔊 课前提示  
> 本章节带大家快速上手使用扣子，通过本章学习，大家可以掌握扣子(Coze)的使用方法。

## 1\. 创建和编排Bot

在界面的左上角，你可以点击"创建 Bot"按钮来创建一个新的Bot。

![](https://www.bzfree.com/upload/images/coze/coze7.png)

## 2\. 设定基本信息和功能

例如，这里我要创建一个帮我写爆款小红书文案的Bot。那么我为这个Bot起名为：小红书爆款写作

![](https://www.bzfree.com/upload/images/coze/coze8.png)

## 3\. 设定大语言模型

这里选择"moonshot(128k)"模型。moonshot是月之暗面的模型，也就是当前很火热的Kimi使用的模型。

![](https://www.bzfree.com/upload/images/coze/coze9.png)

## 4\. 设定人设与回复逻辑

在这里要对Bot的人物进行设定，以及让Bot如何回复用户的问题。这里涉及到提示词如何撰写的知识，我会在后面的章节为大家讲解，如何写出高质量的关键词。

![](https://www.bzfree.com/upload/images/coze/coze10.png)

## 5\. 预览与调试

在快速开始这个章节，我们先不使用插件，工作流等，目的是为了让大家快速上手。这些功能点我们会在后面的章节逐一讲解，要照顾一下从零起步的同学哦 😊  
在这里我提出了一个主题：写一篇华为手机的文案。可以看到Bot快速的帮我生成了文案，质量是相当的高！😍

![](https://www.bzfree.com/upload/images/coze/coze11.png)

## 6\. 发布Bot

Bot创建好以后，我们就可以发布到应用商店供朋友，同事或网友们进行使用了。  
点击右上角的 **发布** 按钮。

![](https://www.bzfree.com/upload/images/coze/coze12.png)

发布之前你可以设置Bot的 **开场白** 和 **预置问题**。

![](https://www.bzfree.com/upload/images/coze/coze13.png)

点击展开，可以对开场白进行预览。

![](https://www.bzfree.com/upload/images/coze/coze14.png)

点击 **确认** 按钮进行发布。

![](https://www.bzfree.com/upload/images/coze/coze15.png)

可以看到，Bot可以被发布到多个平台上进行使用。在这里我们只发布到Bot商店，其他的平台我们在之后的章节里讲解。  
点击 **发布** 按钮进行发布。

![](https://www.bzfree.com/upload/images/coze/coze16.png)

发布成功！ 🎉🎉🎉

![](https://www.bzfree.com/upload/images/coze/coze17.png)

点击 **立即对话**，就可以使用了噢！😊

![](https://www.bzfree.com/upload/images/coze/coze18.png)

> 💡 小结  
> 这一章我们通过对扣子基本功能的使用，相信大家都可以上手使用扣子了。接下来的章节，我为会大家进一步讲解扣子的更多功能，那么就让我们开始吧！

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论**

___

  

## 第三章：插件开发及使用

> 🔊 课前提示  
> 这一章，我们来深入讲解插件的开发及使用。

## 1\. 插件是什么

简单来说，插件是用来增强Bot的能力的，相当于你在玩游戏时，给你的人物加了一个技能。例如你创建了一个Bot，但这个Bot本身是没有上网查找资料的功能的，这个时候你就可以为你的Bot增加一个带有网页搜索功能的插件，那么当你向Bot提问时，Bot就可以先到网上查找资料，再回答你的回答，让回答更实时可靠。

当然，如果你觉得扣子集成的插件不满足您的使用需求，您还可以创建自定义插件来集成需要使用的 API。

## 2\. 使用插件

让我们先从使用一款插件开始，通过使用一款插件，可以让我们了解插件的基本功能和原理。我们继续第一章的示例，为小红书爆款写作助手增加一个上网搜索的超能力。🏄

### 2.1 添加插件

下图所示部分就是Bot的插件。点击 **+** 按钮，我们可以为插件增加一个工具。

![](https://www.bzfree.com/upload/images/coze/coze19.png)

在这里点击 **添加** 按钮，为插件增加一个 **必应搜索** 工具。

![](https://www.bzfree.com/upload/images/coze/coze20.png)

### 2.2 编写提示词

增加插件后，我们需要在提示词里告诉Bot，在回答之前，先使用插件上网进行搜索内容。如下图所示：

![](https://www.bzfree.com/upload/images/coze/coze21.png)

### 2.3 测试插件

接下来测试一下，插件是否被执行了。  
如下图所示，必应搜索 插件已经被执行了。👍👍👍

![](https://www.bzfree.com/upload/images/coze/coze22.png)

可以发现，从网上搜索的内容已经被应用到文章中了。

![](https://www.bzfree.com/upload/images/coze/coze23.png)

> 🔊 敲黑板  
> 使用扣子的重点和难点是，通过提示词让大模型去准确的调用相应的插件。相信通过动手练习，你会很快掌握技能的。

## 3\. 创建插件

> 💡 有些情况下，扣子集成的插件并不能满足我们的需求，那么我们就可以通过创建自定义插件来的方式，集成自己的API到插件中来使用。

### 3.1 初始化插件

点击左侧的 **个人空间**，然后在上面选择 **插件** 标签，点击 **创建插件** 开始创建。

![](https://www.bzfree.com/upload/images/coze/coze24.png)

> 🔊 说明  
> 为了测试方便，我们使用一个线上公开的测试接口。这个接口可以返回文章和文章列表作为演示数据。

> 接口地址：https://jsonplaceholder.typicode.com/

在弹出的页面中，我们为插件填写基本信息。

![](https://www.bzfree.com/upload/images/coze/coze25.png)

插件工具创建方式这里，我们先选择基于已有服务创建，在CozeIDE中创建的方式我们之后再讲解。

插件URL 这里重点注意一下，这里需要填写接口的根域名。

![](https://www.bzfree.com/upload/images/coze/coze26.png)

接下来解释一下授权方式这个选项。

![](https://www.bzfree.com/upload/images/coze/39eca87c-336e-4bc8-a225-00aecfb06be6.png)

授权方式有三种：不需要授权、Service 和 Oauth。

不需要授权：就是无认何认证环节，请求接口，接口返回值。

Service：服务认证，该认证方式是指 API 通过密钥或令牌校验合法性。就是你要向接口传递令牌信息，后端验证成功才能给你返回值。

OAuth: OAuth 是一种常用于用户代理身份验证的标准，它允许第三方应用程序在不共享用户密码的情况下访问用户下的特定资源。

> 🔊 说明  
> 如果有想了解OAuth机制的，推荐看阮一峰老师的讲解，通俗易懂。  
> https://www.ruanyifeng.com/blog/2014/05/oauth\_2\_0.html

这里我们使用 不需要授权 做演示。

填写好信息以后，点 确定 按钮，就完成了插件的设置。

![](https://www.bzfree.com/upload/images/coze/coze27.png)

接下要开始在插件中加入工具了。

![](https://www.bzfree.com/upload/images/coze/coze28.png)

### 3.2 填写基本信息

![](https://www.bzfree.com/upload/images/coze/coze29.png)

### 3.3 配置输入参数

点击 新增参数 按钮为接口增加一个参数。  
因为我们使用的接口地址是：

> 🌐 https://jsonplaceholder.typicode.com/posts?id=2

所以参数名称那里我们填写的是id。

![](https://www.bzfree.com/upload/images/coze/coze30.png)

传入方法这里说一下，一共有四种：

Body：就是参数放在请求体中的请求。

Path：就是参数作为URL中的一部分。例如下面这个URL，todos参数就是path中的一部分。  
https://jsonplaceholder.typicode.com/posts/2

Query：参数作为URL中的参数，例如下面这个URL。  
https://jsonplaceholder.typicode.com/posts?id=2

Header：就是在请求头中传递。

点击 **保存并继续** 按钮，进入下一步。

![](https://www.bzfree.com/upload/images/coze/coze31.png)

### 3.4 配置输出参数

点击 **自动解析** 按钮

![](https://www.bzfree.com/upload/images/coze/coze32.png)

我们访问这个接口，可以看到，会返回以下参数。

> 🌐 https://jsonplaceholder.typicode.com/posts?id=2

那么这里我们把id的值设置为2，点击 自动解析 按钮。看自动解析的结果和上面的结构是否一样。

![](https://www.bzfree.com/upload/images/coze/coze33.png)

可以看到解析出来的字段和上面代码块中的字段完全一致，说明解析没问题。

![](https://www.bzfree.com/upload/images/coze/coze34.png)

继续下一步，点击 **保存并继续** 按钮。

### 3.5 调试与校验

把id值设置为2，点击 **运行** 按钮，查看 **Response** 结果。

![](https://www.bzfree.com/upload/images/coze/coze35.png)

可以看到和上面代码块中的值一致，说明返回结果没问题。

点击 **完成** 按钮，此时插件就创建完成了。

![](https://www.bzfree.com/upload/images/coze/coze36.png)

从上图可以看到，服务状态是 **线下**，这时插件虽然已经创建好了，但还是不能被Bot调用的。

我们需要对插件进行发布以后才能被Bot使用。

## 4\. 发布插件

发布插件很简单，点击 **发布** 按钮即可。

![](https://www.bzfree.com/upload/images/coze/coze37.png)

发布完成前，需要确认你发布的插件是否会收集、传输用户的个人信息，请如实填写。因为这里是案例教程，我们就直接发布了。

![](https://www.bzfree.com/upload/images/coze/coze38.png)

此时可以看到，插件已经是 **已发布** 状态了。

![](https://www.bzfree.com/upload/images/coze/coze39.png)

接下来在Bot中添加插件的时候，在左侧选择 **我的工具**，就可以看到我们刚才创建的插件了。

接来了就可以按照 **插件使用** 教程的方法来使用插件了。

![](https://www.bzfree.com/upload/images/coze/coze40.png)

## 5\. 导入插件

有的同学可能会问，每次创建插件都需要按照 **创建插件** 的流程写一遍吗？

如果想把已经创建好的插件导入到另一个帐号使用，或者想在已经创建好的插件的基础上稍做改动就可以变成一个新的插件，有没有更简单的方式？

答案是有的。我们可以使用 **导入插件** 的功能。

例如，我们要基于刚才创建好的插件，把工具的名称修改一下，变成一个新的插件，我们可以按以下方式去做。

### 5.1 复制代码

进入我们刚才创建好的插件

![](https://www.bzfree.com/upload/images/coze/coze41.png)

点击 **使用代码** 按钮

![](https://www.bzfree.com/upload/images/coze/coze42.png)

可以看到弹出的这个代码界面，我们全选复制右侧这个Yaml格式的代码，把它先放到一个临时的文本文档中进行修改。

![](https://www.bzfree.com/upload/images/coze/coze43.png)

### 5.2 修改文件

在文档中修改一下插件名称和工具名称。注意插件名称仅支持输入中文、字母、数字、下划线或空格，不能有特殊符号

![](https://www.bzfree.com/upload/images/coze/coze44.png)

### 5.3 保存YAML

把文件进行保存，起一个文件名，例如new\_plugin.yaml，这个名称随意写，注意一下扩展名是yaml。

> 💡 名词解释  
> 简单来说yaml是一种文件格式，使用空白符号缩进等格式，使文档格式有层级递进关系，使文档更易读易写。我们当前复制出来的这段代码就是yaml格式的，所以扩展名也要用yaml。

### 5.4 导入文件

点击 **导入** 按钮

![](https://www.bzfree.com/upload/images/coze/coze45.png)

选择我们刚才创建的 new\_plugin.yaml 文件进行导入，然后点击 **下一步** 按钮。

![](https://www.bzfree.com/upload/images/coze/coze46.png)

可以看到插件名称和我们修改的一致，说明导入没问题。点击 **确认** 按钮继续。

![](https://www.bzfree.com/upload/images/coze/coze47.png)

### 5.5 调式与效验

确认之后，我们发现调试状态是失败的，如下图所示。

![](https://www.bzfree.com/upload/images/coze/coze48.png)

这个时候我们需要启用，然后重新调试一下就好了。

![](https://www.bzfree.com/upload/images/coze/coze49.png)

按之前 **调试教程** 的方式调试后，点击 **完成** 按钮。

![](https://www.bzfree.com/upload/images/coze/coze50.png)

可以看插件已成功导入了。

![](https://www.bzfree.com/upload/images/coze/coze51.png)

> 💡 小结  
> 这一章我们通过扣子插件的创建、使用、发布和导入等内容进行了讲解，相信大家都可以熟练的使用扣子的插件功能了。接下来的章节，我为会大家进一步讲解扣子的更多功能！

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

  

## 第四章：知识库创建及使用

## 1\. 什么是知识库

大语言模型的训练数据一般基于公开的数据，这意味着模型的知识**一般不会包含私有领域的知识**，同时在公开知识领域**存在一定的滞后性**。为了解决这一问题，目前通用的方案是采用 \*\*RAG（检索增强生成）\*\*技术，**使用用户问题来匹配最相关的外部数据**，将检索到的相关内容召回后作为模型提示词的上下文来重新组织回复。

扣子提供了一套简单易用的用户界面来方便应用构建者管理个人或者团队的知识库，并能够快速集成至 AI 应用中。你只需准备文本内容，例如：TXT、DOC、DOCX、Excel、PDF 文件，甚至在线网页、飞书文档、Notion页面是也可以的。

![](https://www.bzfree.com/upload/images/coze/d9AkEAtO2yn5XiOoqUizmbDtm12fBRmXidZs8eqiWv4.png)

## 2\. 创建知识库

**下面我们写一个示例，例如FuturaTech是一家企业，那我们来为这个企业做一个FAQ。**

点击 **创建知识库** 按钮，开始创建。

如下图所示位置：

![](https://www.bzfree.com/upload/images/coze/yyH_UJNQlGGj0_KnEVWzcQl2KrfP4kF49EMopoSp7c8.png)

这个知识库我们使用文本格式来创建。例如FuturaTech是一家企业，那我们为这个企业做一个FAQ Bot。

![](https://www.bzfree.com/upload/images/coze/FkZjjPun4ekcUcImeELI5MxQ8SDdfsutl-ZrlowB9jg.png)

**准备文档**

首先，我们准备一个FAQ的文本文档，用TXT格式就可以，例如文件名叫：FAQ.txt。

文本内容如下：

**上传文档**

在这里，把文件进行上传，然后点击 **下一步** 按钮：

![](https://www.bzfree.com/upload/images/coze/-tquJMNXd3d6XeEy2gZiXxCaeYNt3YSACSkGQRAA-QU.png)

**分段与清洗**

这里注意一下，内容分段可以更有效地召回与用户查询最相关的内容，从而提升回复的准确性。合理的内容分段对回复的效果有着直接影响。一般没有特殊要求的情况下，我们这里选择 **自动分段与清洗** 即可。

点击 **下一步** 按钮：

![](https://www.bzfree.com/upload/images/coze/wK6BCMWKUv1GfU2t4_kCUL67KCe1GFU5kIWKzOdM6lA.png)

这里服务器开始处理，点击 **确认** 不影响数据处理，处理完毕后可进行引用。

![](https://www.bzfree.com/upload/images/coze/pMuBU9dHxq-j6pVHzwQkYrvLWNszt4gYRWmi1zr0yKw.png)

处理完成后，可以看到分段后的内容：

![](https://www.bzfree.com/upload/images/coze/LB4Pq_dY3q_TB3shCemiE234sV9JmNg3M5TVLNYbVho.png)

到此我们的知识库就创建完毕了。

## 3\. 使用知识库

  

### 3.1 创建Bot

我们通过创建一个Bot来引入知识库。

![](https://www.bzfree.com/upload/images/coze/17Fx4b435pZqik7Z3AF3cz6vFJkLnPNgmRj27hjov1g.png)

### 3.2 **添加知识库**

点击 **+** 添加之前建好的知识库

![](https://www.bzfree.com/upload/images/coze/JUxpIzHvOANal1VPAG2qjDxJBmJqOQl4doqKC6pjbcQ.png)

**选择知识库**

在知识库列表中搜索FuturaTech关键字，点击 **添加** 按钮

![](https://www.bzfree.com/upload/images/coze/xr-hwuLRFHqpxZ8AM0JwP9XzMkuU9puK1rZXjDMzCr8.png)

### 3.3 **设置知识库**

加好知识库后，要对知识库进行一下设置。

![](https://www.bzfree.com/upload/images/coze/VQhyTNAfV9ytGOaUvSNNN1Y2EWv194W_T3DOiPW-cf0.png)

1.  **调用方式**

分别解释一下，调用方式这里 **自动调用** 和 **按需调用** 是什么意思。

\*\*自动调用：\*\*是指每一轮对话都会调用知识库，使用召回的内容辅助生成回复。

**按需调用**：是指根据实际需要来调用知识库，使用召回内容辅助生成回复。此时，需要在左侧的人设与回复逻辑区域明确写清楚在什么情况下调用哪个知识库进行回复。

2.  **搜索策略**

搜索策略是用来选择如何从知识库中搜索内容片段，不同的检索策略适应于不同的场景。检索到的内容片段的相关性越高，大模型根据召回内容生成的回复的准确性和可用性也越高。

\*\*混合：\*\*结合全文检索和语义检索的优势，并对结果进行综合排序召回相关的内容片段。

\*\*语义：\*\*像人类一样去理解词与词，句与句之间的关系。推荐在需要理解语义关联度和跨语言查询的场景使用。例如下面两组句子，第一组的语义关系就更强。

\*\*全文：\*\*基于关键词进行全文检索。推荐当查询内容包含以下场景时使用

-   特定名称或专有名词，术语等，例如比尔盖茨、 特斯拉 Model Y
    
-   缩写词，例如 SFT
    
-   ID，例如，12s1w1s2系列
    
    基于以上的理解，这里我们设置如下图所示：
    

![](https://www.bzfree.com/upload/images/coze/topUgCqujkPc0YTzVIk8rc2nK2vyW2IqzVdpd_9qyg8.png)

### 3.4 编排提示词

接下来设置Bot的 **人设与回复逻辑** 部分\*\*，告诉Bot当客户出问题的时候先到知识库中查找答案。\*\*

![](https://www.bzfree.com/upload/images/coze/LPRL_doVsNAF0UgkJNq4MpKhMTRA8jyremvbAoKfAgI.png)

提示词：

### 3.5 **预览与调试**

接下来我们来测试一下，当我们问Bot问题，Bot是否调用了知识库。

我找到了一条 FAQ.txt 中的问题。

![](https://www.bzfree.com/upload/images/coze/BnLszlUk22zOUIbRKK2NfrPS9_f0ZJjupEa6iCEUNSs.png)

如下图所示，可以看到，Bot调用了知识库并正确的回答了问题。

![](https://www.bzfree.com/upload/images/coze/eahlyx1UwHmYQzqg3YBEPsVLA6-ql8kve9r0RAoADcY.png)

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

  

## 第五章：工作流创建及使用

## 1\. 什么是工作流

工作流是可以让用户能够通过**直观的方式**，**灵活地组合插件**、**大型语言模型和代码模块等元素，构建出既复杂又稳固的业务的流程。** 这在执行如旅行规划、报告分析等任务时尤为有效。当面临包含多个步骤的任务场景，并且对输出结果的精确度和格式有着严格标准时，采用工作流配置将是一个理想的选择。

## 2\. 工作流的组成

如图中所示，工作流是由多个节点组合而成的一整套流程。\*\*节点是组成工作流的基本单元。\*\*例如，插件节点、大语言模型 LLM、自定义代码、判断逻辑等节点。

工作流默认包含了**开始节点**和**结束节点**。

开始节点是工作流的起始节点，可以包含用户输入信息。

结束节点是工作流的末尾节点，用于返回工作流的运行结果。

![](https://www.bzfree.com/upload/images/coze/coze52.png)

## 3\. 节点示例详解

  

### 3.1 插件节点

与第三章所讲类似，之前讲的是插件直接放到Bot中，通过Bot直接进行调用。而在这里是作为工作流的一个节点，但他们的功能都是一样的，可以访问实时数据和执行外部操作，例如通过搜索引擎搜索信息、图片、时实翻译等。

![](https://www.bzfree.com/upload/images/coze/cvViSx8ED90vSOHWdn.png)

**下面我们写一个示例，来获取知乎列表的热榜。**

因为知乎热榜只有一个limit参数，用来获取条数的。这个数量我们让用户来设置。

点击 **试运行** 测试：

![](https://www.bzfree.com/upload/images/coze/coze54.png)

输入数量

![](https://www.bzfree.com/upload/images/coze/coze55.png)

查看运行结果，知乎热榜数据已经调用成功了：）

![](https://www.bzfree.com/upload/images/coze/coze56.png)

### 3.2 大模型节点

可以调用大语言模型，使用变量和提示词来**回答用户的问题或对上一个节点的内容进行分析和总结**。

![](https://www.bzfree.com/upload/images/coze/coze57.png)

**下面我们写一个示例，用大语言模型来润色用户的文字。**

这里的**模型**我们可以任意选择，我选择的是是通义千问-Max；然后为输入参数起一个变量名text；

注意提示词那里，要引用输入参数text的时候，需要**{{text}}**这样写。

我们这里写的是：**请润色一下用户的给的文字：{{text}}**。这样大模型就能理解我们的指令去润色text文字了。

具体设置如下图所示：

![](https://www.bzfree.com/upload/images/coze/coze58.png)

试运行一下，看看结果：

![](https://www.bzfree.com/upload/images/coze/coze59.png)

输入"外面的景色真好"，点击 **运行** 按钮。

![](https://www.bzfree.com/upload/images/coze/coze60.png)

查看运行结果，可以看到大模型为我们润色的还是不错的：）

![](https://www.bzfree.com/upload/images/coze/C4XACGyv5QOhOK74TtOr9fGq2IYs1LJY13pvUr-OUz4.png)

### 3.3 代码节点

代码节点是用来编写代码，处理输入变量来生成返回值

通过以下这个示例，大家可以一目了然的明白代码节点的作用。用最简单的示例解释了代码节点每个参数的作用，请注意绿色线所标注的各变量之间的对应关系。

![](https://www.bzfree.com/upload/images/coze/Cv5s61qMrx0zh1SiMnc0tlvBGpJbfB5_ViRt0YGxAVo.png)

**编写代码**

点击 **在IDE中编辑** 可以编写代码

![](https://www.bzfree.com/upload/images/coze/JL5lwiulCVY6ox-ofpqMQ1Fx-DXVyZ4NcpzKYKBm3HM.png)

这个示例代码的作用是：为用户请求参数加一个叹号" ! "，也就是做一个字符串拼接的功能，然后返回新的值。

注意params对象中的值，对应的是输入参数，如果下图所示：

![](https://www.bzfree.com/upload/images/coze/3v8IhdCEoDYNRyR3hW7ymEfjr4uO6JRxiExu1UYSqbo.png)

点击 **测试代码**：

![](https://www.bzfree.com/upload/images/coze/5mulVWY4zXhNZgSvGaueWrJPmf748utBi2n8CBn8XHk.png)

按图中所示三步进行测试：

![](https://www.bzfree.com/upload/images/coze/badLfbxkqDhHaYALbgdOCtZHxK1w1yRn5vTdWDVTlVo.png)

点击 **确定** 按钮。

![](https://www.bzfree.com/upload/images/coze/2BjrVLaiAgDrMHqRk6D5Zv4PJzOjXJ7_liu0E--nZh0.png)

作用是把代码中返回的key值，作为输出的key值，以便为了下一个节点使用。

![](https://www.bzfree.com/upload/images/coze/ob1SSQx6jYPHIWQVuSmJEMOdnSLXuetg5ET-NelQo7s.png)

接下来 **试运行** 一下。

![](https://www.bzfree.com/upload/images/coze/LwQ6eyXqbg9MhKOWGx4tUnbiRrxuDDymG8-1J-JqW-w.png)

输入"你好啊"，期望输出"你好啊！"，点击 **运行** 按钮。

![](https://www.bzfree.com/upload/images/coze/R6QXB9suHyP26dsUWomXpiHmmuoiZE1liFBUXbiinn4.png)

**输出结果**

可以看到，是我们期望的结果了 😊

![](https://www.bzfree.com/upload/images/coze/UUeoZGcoNgP07VdkAzAQPdKWaLEN6GQXOpxzgdOcO4Y.png)

### 3.4 知识库节点

与 [第四章：扣子知识库使用](https://www.bzfree.com/coze/#%E7%AC%AC%E5%9B%9B%E7%AB%A0-%E7%9F%A5%E8%AF%86%E5%BA%93%E5%88%9B%E5%BB%BA%E5%8F%8A%E4%BD%BF%E7%94%A8 "扣子知识库使用")， 所讲类似，之前讲的是直接在Bot中引用知识库，通过Bot直接进行调用。而在这里是作为工作流的一个节点，但他们的功能都是一样的，在选定的知识中，根据输入变量召回最匹配的信息，并以列表形式返回。

**下面我们写一个示例，我们还是以第四章中FuturaTech的FAQ咨询为例，写一个工作流，用知识库增强回复的准确性。**

首先看一下下面这个图，在这个示例里，**有一个地方要注意一下，和之前的示例有一些区别。**如果我们要使用知识库，还要**借助一个大模型节点**，这个大模型节点的作用是：对根用户提问和知识库节点匹配的内容进行重新组合，生成符合提示词要求的内容，返回给用户。

![](https://www.bzfree.com/upload/images/coze/8BZrGiHQucKDNkhVR1bS1kbsdLYkogmYh7I5C7VcBxM.png)

**添加知识库**

点击 **+** 添加知识库：

![](https://www.bzfree.com/upload/images/coze/AdECyTSBjZN1AB43pw54jYu-OKVzNG10Bw7lC-0LTuI.png)

选择之前创建好了的知识库，点击 **添加** 按钮：

![](https://www.bzfree.com/upload/images/coze/OhdSveS2D2_UpQGiAjz90xYBBqvFf0QP7LZ2V7jBF6k.png)

**设置大模型节点**

大模型节点这里，模型这里我使用的是通义千问。模型可以任意选择，在调试的时候可以都测试一下，看哪个效果好就用哪个。要注意的地方是 输入参数 这里，从图中可以看到，引入了两个参数，一个是question，一个是knowledge，分别对应的是用户的提问和知识库节点的输出。

![](https://www.bzfree.com/upload/images/coze/ic3sGLMyQf7gTvibwpmD2SHgI1q7uKs75oOciEsyNm4.png)

**设置大模型提示词**

有了这两个变量，接下来我们要结合这两个变量去写提升词。这里也不需要有一个固定的写法，只要把你想要的结果，通过描述告诉大模型就可以了，下面是我写的一个提示词，大家可以在此基础修改成自己的。

具体如下图所示：

![](https://www.bzfree.com/upload/images/coze/XHL-IZanZmqlrLjjc3FmU8Phc0C6C4jioP7GpYUQA8c.png)

**预览与调试**

如图所示，点击试运行：

![](https://www.bzfree.com/upload/images/coze/FccKnGNi1dZ7VDWC-v-_j1XDrl9qlbMObYmUh9LkTEo.png)

输入问题

![](https://www.bzfree.com/upload/images/coze/y8Ehexmp7j7o7x1J7ykAp-NlMv9SVo4sRWx7umfVLHo.png)

查看结果

![](https://www.bzfree.com/upload/images/coze/f4ew7fgrQ4tF4SNbGXA9UOBGlnf_4doo8_-PMpT3DEs.png)

可以看到，是我们期望的回答结果了 😊

### 3.5 选择器节点

选择器节点是连接多个下游分支，若设定的条件成立则仅运行对应的分支，若均不成立则只运行“否则”分支。

通过以下这个示例，大家可以一目了然的明白选择器节点的作用。用最简单的示例解释了选择器节点每个参数的作用。

我们通过以下这个示例，来解释了 **选择器节点** 分支的作用。

示例所期望的效果是：当用户的输入值为1时，执行**消息一**的流程；当输入其它值时，执行消息流程。

流程的结构如图所示：

![](https://www.bzfree.com/upload/images/coze/Z0J2Jcoz-xd9NzxNrRhQjq9hE4H3SKc3v7yDiQEgmJw.png)

当用户输入的参数为 1 时：

![](https://www.bzfree.com/upload/images/coze/0xoZTtqnW_shQWfs-qVVCrGEJtRJpAX1aSO_-52Z2a0.png)

可以看到运行的是上面 **消息一** 的流程：

![](https://www.bzfree.com/upload/images/coze/uRvb8PFF4A2nXDyRfBe-ol7lR55xZpFXhAtJxE5MD-g.png)

当用户输入的参数为 2 时：

![](https://www.bzfree.com/upload/images/coze/HJXlz_1GWlSLxcn6q1OO4PRu6y3eb-BFUTP8LHbBba0.png)

可以看到运行的是上面 **消息二** 的流程：

![](https://www.bzfree.com/upload/images/coze/psS8gZ8xmjTYIfB7pDxvMvWZ91JRjZeqoOD-d8Yl5b0.png)

可以看到，是我们期望的回答结果了 😊

### 3.6 消息节点

消息节点是支持中间过程的消息输出，支持流式和非流式两种方式。

下面我们通过一个示例，来看一下消息节点的作用。

这个示例是：当用户输入一个漫威人物，大模型会对输入的人物进行介绍。这里要注意的是，消息节点在这里的作用是：在大模型输出结果之前，提示用户"下面为大家介绍一下漫威人物XXX"。

这里要注意一下，如果要单独调试消息节点不容易看到效果，这里我们要借助一个大模型节点来观察效果。

![](https://www.bzfree.com/upload/images/coze/ElVvor8ac1LuNY-X9RPzhIpDt3EBGd1ez5_3MvzgR8g.png)

试运行一下，我们在输入参数中输入：钢铁侠。

![](https://www.bzfree.com/upload/images/coze/NNsuxShrixNd5uzlY1f-HI1aWOJLNzvbw0GDYYpb0-s.png)

这个图可以看到，当大模型节点正在运行的时候，消息节点已经输出了内容："下面为大家介绍一下漫威人物-钢铁侠"，**这个过程放在实际场景中是在让用户等待大模型输出结果。**

![](https://www.bzfree.com/upload/images/coze/N_BUtL4rL2oYsUgFRcoX4IA-xwMuglrTtlSY_J7YG0g.png)

下图可以看出，在消息结点运行完几秒之后，大模型才输出结果。

![](https://www.bzfree.com/upload/images/coze/lCO-MUhDIXtZlLTvNn8Tn3xDyjuYjVFUx2GW_9JHMV0.png)

这就是消息节点的作用。在之后工作流使用过程中，我们还会看到消息节点更实用的作用。😊

### 3.7 工作流节点

工作流节点是集成已发布好的工作流。也就是把之前发布好的工作流当做一个子任务，嵌套子在任务流中执行。

![](https://www.bzfree.com/upload/images/coze/YWJtU8n_USSjeKtYdpGFq8oiDsjLQepIfZ9ULDEOdmU.png)

下面我们通过一个示例，来看一下**如何在一个工作流里嵌套另一个工作流。**

我们把 3.6 消息节点 中讲的示例发布一下，把这个3.6的示例当成一个子任务。放到我们本节这个示例中演示。

这里先提一下，工作流节点，只有发布以后，才能被使用。

如下图所示，先把工作流进行一下发布，点击 **发布** 按钮即可。

![](https://www.bzfree.com/upload/images/coze/6Bwp4Wnakf4_SY6CbaS4xZ0E9N5jlOJo7sDrCMHUcZo.png)

可以看到，很简单就发布成功了。

![](https://www.bzfree.com/upload/images/coze/chyLnOcHSswmywZkoujw_TRvnoyuWqALBk65kyJ-hn0.png)

接下来我们再创建一个工作流，点击 **创建工作流** 按钮。

![](https://www.bzfree.com/upload/images/coze/9SSwAOgP5GKVD2yKj1mZXV5LOlYvgKJmzSe9iNZPDSw.png)

为工作流节点起一个名称和描述，然后点击 **确认** 按钮。

![](https://www.bzfree.com/upload/images/coze/X_x4b5W9EXl59PB1q5kVsjVLEtqO7bhe5CSaFoLkufc.png)

点击 + 添加一个工作流。

![](https://www.bzfree.com/upload/images/coze/Ia3aK1CuF0O2mpETTYN5EIjcptNs-SLla25e7U4Ydr8.png)

点击 **添加** 按钮。

![](https://www.bzfree.com/upload/images/coze/8uIdsRkctNyistOJdvVZPgbYG7m1ZLqC_g2Ab_MpZfI.png)

这样就把消息流节点添加进来了。

![](https://www.bzfree.com/upload/images/coze/zItJBfqYeUiiaZzvDcuE0eSNSJtkmTV1axSO4qhNiQc.png)

接下来我们进行一下测试，把3.6节点，用户的输入替换成当前TestCallMessageNode工作流的query参数。

![](https://www.bzfree.com/upload/images/coze/PwubnM8wmPVITSOAeH3L0LXfXAeejn3XwTQD2oP2hGg.png)

接下来进行一下测试。点击 **试运行** 按钮。输入参数和3.6节所讲一样，还是填入"钢铁侠"，然后点击 **运行** 按钮。

![](https://www.bzfree.com/upload/images/coze/oaSKTmc7M_TGhWIACGJElJ5MUmohv90_LZ32Kq5__2o.png)

如下图所示，和我们期望结果的一样。我们在 **TestCallMessageNode** 工作流中调用了 MessageNodeWorkFlow，MessageNodeWorkFlow同时作为**TestCallMessageNode** 一个嵌套的子任务，我们得到的结果和3.6节的结果是一样的。😊

![](https://www.bzfree.com/upload/images/coze/tmPuSmLgIdCBoSqZYbnZM5F2YDgkTFUqxqJGB-RfJmw.png)

### 3.8 变量节点

变量节点是用于读取和写入Bot中的变量。**变量名称必须与机器人中的变量名称相匹配。**

![](https://www.bzfree.com/upload/images/coze/_DFKlHU2y9tasjjgz1sLYypFOnuXakCvX9ed_8iq_xY.png)

我们通过一个示例，如果配合Bot来使用变量节点。

通过变量节点的定义，可以知道：使用变量节点之前要有个前提，就是**首先要有个Bot，并且这个Bot里定义了一变量，否则单独使用变量是没有意义的。**

所以首先，按创建第二章的方法，先创建一个Bot。

![](https://www.bzfree.com/upload/images/coze/akXDuS54fPYB2FPnJrjINSVLGBt8-PezxU6-O2B06Ts.png)

点击 + 按钮添加变量。

![](https://www.bzfree.com/upload/images/coze/eKltTn3wSwfNMSHjWLXMOPUiLc_jn9RjjSzOI-NXXLI.png)

定义一个变量role，来表示漫威的人物

![](https://www.bzfree.com/upload/images/coze/HvpYS5OmytdEtB7k2UptJPU1M7oGDzDYRwo-LMPec9M.png)

接下来发布一下。

![](https://www.bzfree.com/upload/images/coze/0oB7XOkrIkAVeAl2owUlDbq_feGHwDJaJkzHNyoQ964.png)

接下来创建带节点变量的工作流。

如图所示，创建了两个变量节点。第一个节点是使用用户的输入值来设置变量role(和Bot中的变量对应)的值，第二个节点是用来获取变量role的值。最后使用role的值输出。

同学们按如下图的方式进行创建。注意红框所标准的位置设轩

![](https://www.bzfree.com/upload/images/coze/mGWmDLdodifobLK6eWQX_7DiG1P_IyMh2Q77fzTZ1R8.png)

细节大图：

![](https://www.bzfree.com/upload/images/coze/qg1jC9vNuAlBJWPnuxipQDpIpkWr8kiFxjhPK-uXfpo.png)

设置好以后我们运行一下。

![](https://www.bzfree.com/upload/images/coze/Iauvyby0d71dyvJyiEihvy-JTGKJVOQllxWZrYIHXZI.png)

可以看到这里就要求我们关联之前创建的Bot了。

![](https://www.bzfree.com/upload/images/coze/cgheH8WkCI0WXz6RCv8gKS2QF0xWbfzjdj6OgWKHwFE.png)

选择后点击运行，查看结果。

![](https://www.bzfree.com/upload/images/coze/nKxVPUAbEJFfDcvAmO2qamNe2dVFnh9YMeDzlDnKR8E.png)

可以看到，成功输出了我们在上一步上设置的role变量的值。😊

### 3.9 数据库节点

简单来说，数据库是用来存储数据的。那 **数据库节点** 就是在工作流中存储数据的。扣子中的数据库支持放开读写控制，用户可读写其他用户提交的数据。权限由开发者控制。**需要提前在 Bot 的 Database 中添加 Table。**

![](https://www.bzfree.com/upload/images/coze/2b9Dkqci-vjhlunhm2TtYO6pY7O1vHncQufXx-Y8yB8.png)

我们通过一个示例，如果配合Bot来使用数据库节点。

通过数据库节点的定义，可以知道：数据库节点和变量节点一样。使用之前要有个前提，就是**首先要有个Bot，并且这个Bot里已经创建了数据库，否则是读取不了数据的。**

所以首先，按创建第二章的方法，先创建一个Bot。

![](https://www.bzfree.com/upload/images/coze/MtXWbiWdu4-WLIUSTlL0mBw10eG4VrgDzTVTTchsL9Y.png)

点击 + 添加一个数据表。

![](https://www.bzfree.com/upload/images/coze/7SSRq1mvLdyAmBmPx3JwFJ6ta6WKonUoGrYHaERerc8.png)

为数据表新建字段。

![](https://www.bzfree.com/upload/images/coze/bx6LOxaQAP4XZAB4BdvVRApfH3cc1FdutZPOE02iBYQ.png)

为了演示方便，我们使用模板进行创建。点击 使用模板 按钮。

![](https://www.bzfree.com/upload/images/coze/-VZmJf9p4jPnV9BdHu6UN-C4pQrzkZhAhbYlsJ5UgII.png)

可以看到，模板建了一个"用于保存读书笔记"的数据表。数据表的名称、描述和字段都已经建好了。点击 保存 按钮。

![](https://www.bzfree.com/upload/images/coze/Zv40K_tZklEaHEFlJehg8MhFKl9UVcrNJbQmb0GiFsU.png)

可以看到数据表已经创建好了。

![](https://www.bzfree.com/upload/images/coze/c7Jad-o27BgreboAnuY4HIwhdfCkrjWB0-YjWfWQwlQ.png)

我们来演示一下如何向数据表中插入数据。

向数据库中插入数据，不需要你学习复杂的SQL语言。通过自然语言与 Bot 进行交互，即可插入或查询数据库中的数据。

如下面这个示例：

![](https://www.bzfree.com/upload/images/coze/CsP99TyLmcdedv49DzojfVtYtUne305xjfDVBpDsHzY.png)

可以看到，我只是简单的告诉Bot："三国演义这本书很精彩"，Bot就帮我把这本书记录到数据库中了。

再来测试一下查询功能，从下图可以看出，Bot很容易的给出了答案，只有一本我们刚刚插入的《三国演义》这本书。

![](https://www.bzfree.com/upload/images/coze/zUpBvoPWLhJ95rcjnpvEZnYjwK619C5VmZWoKWA6_3Q.png)

到这里，数据表的建立就完成了。

在这个示例中，我们想实现的效果是：先在数据库中插入一条数据，然后再查询数据表，验证是否插入成功。

![](https://www.bzfree.com/upload/images/coze/ManoNln5kZbxkgY1mrDOFxMSc4YmJKJDycKI6eWlMHE.png)

如果你会写SQL也没关系，我们使用 **自动生成** 的功能，在查询目标里输入自然语言描述我们想要的操作：例如"向book\_notes表中插入一条数据"，然后点击 自动生成 按钮，就会成生一条SQL语句。点击 **使用** 按钮，SQL语句就被应用了。

![](https://www.bzfree.com/upload/images/coze/bCSgXwQGFBxU1cFezAOzzjYc1YlfnPvCaM4lVWMs94c.png)

这里注意一下，生成完SQL之后，我们需要调整一下这个SQL。生成后的SQL语法是没有问题的，但没有传实际的值，我们要把我们想传的值放到这个SQL中。调整后的效果如下，{{name}}对应的输入参数的name：

![](https://www.bzfree.com/upload/images/coze/B2Nq9AYaBp-xIzcSCztapoXZgaOCy8824GnO7V_p5Kw.png)

试运行，看一下效果：

![](https://www.bzfree.com/upload/images/coze/I4sKCSs8V2YdPfcNMv436IOpkg4xFQzZeTpNR7Wt5uU.png)

如图所示产，流程执行没问题。

![](https://www.bzfree.com/upload/images/coze/uozyEpBFikM9rxfkVoHpValGybLPlSeUb8SAXnmt-Hc.png)

接下来用同样的同样的方法，我们把插入SQL改为查询SQL，来验证一下，数据是否被插入到了数据表中。

如图中标示箭头的位置要注意一下，这里的name要和查询的字段对应，当然你还可以加更多的字段，这里只要一个作为演示。

![](https://www.bzfree.com/upload/images/coze/fCzmkijE-SVobyXGOxfxcBblDeQpB2hB-joYvxEFLBk.png)

可以看到，数据被成功查询出来了。😊

![](https://www.bzfree.com/upload/images/coze/iwzt-1a7wwWAvvsjuBgxQq6o1PqgUnKpbIDEkRydmdc.png)

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

## 4\. 工作流案例讲解

本节开始，我要创建一个工作流。结合之前学过的知识，做一个**图书管理工作流**给图书馆的管理员使用。这个工作流的作用是：通过判断图书管理员指令的意图，来执行对应的操作。

我们期望的效果是：当图书管理员输入类似“请帮我查询有哪些书籍”的时候，工作流就返回当前数据库所有的图书。当输入“向数据库录入一本书”的时候，就向数据库加入一本书。当然也可以通过指令删除。

通过上面的分析，我们可以知道：

1、如果要分析用户的意图，我们要需要使用的节点是大模型节点。

2、判断意图后，我们要执行哪个操作，是查询还是添加，还是删除，这里我们要用到选择器节点。

3、要向数据库中录入书籍，肯定是还需要有数据库节点了。

接下来让我们创建这个工作流。

### 4.1 创建Bot

![](https://www.bzfree.com/upload/images/coze/L_4N5n_ola5JrsV7QeOa4yIRofrbMTP9s7iBX9cxDkw.png)

### 4.2 创建数据表

![](https://www.bzfree.com/upload/images/coze/wmUR4WKEXKaahAU3gMhgQNS-_u356xQuWtqrGRCHkLM.png)

### 4.3 添加字段

![](https://www.bzfree.com/upload/images/coze/s6R_8uVpXQcg5uAQ-X1q3WAeG-z9Ft0wE5iolIPioWU.png)

### 4.4 创建工作流

进入工作流管理页面，点击 **创建工作流**

![](https://www.bzfree.com/upload/images/coze/ptc8A_Ofad5RJzhEif8O6HVtQmeVogIIR2r8zdea748.png)

### 4.5 填写工作流信息

![](https://www.bzfree.com/upload/images/coze/m7x1iD7xoW2hcQaqdweTsx0FQjvlq8TyEMbIdgXGW-g.png)

**我们首先把需要用到的节点先加到视图里，然后再对节点一一进行具体的设置。**

**整体效果预览**

先来看一下最终配置好的整体效果，我们再来一一添加节点到视图中：

![](https://www.bzfree.com/upload/images/coze/kh73jdmBRCQmgBOjvQaBFdoUOAoiJEvEg1rRZUimjhw.png)

### 4.6 添加大模型节点

先添加 **两个大模型节点，**为了更直观的演示流程，这里用两个大模型来分别返回 **图书名称** 和 **操作类型**。（正常情况下，一个大模型节点也是可以搞定的，返回一个**数据对象**即可，这里大家要理解就可以了。）

![](https://www.bzfree.com/upload/images/coze/OevM2pJkwdln2IL-s9ZRUH0bfZ_HoBNesuSLkAxZGYI.png)

### 4.7 添加选择器节点

添加 **两个选择器** 节点，先忽略配置。

![](https://www.bzfree.com/upload/images/coze/GWlp3fFNN5OivuEeJWg-lja1CTkeTdiYxHkNRjyNYHk.png)

### 4.8 添加数据库节点

添加**三个数据库节点**，分别用来查询，添加和删除

![](https://www.bzfree.com/upload/images/coze/yJxe-dzUGYZKH8yCp_64AWfuYwtsyBEi7j149Kp9ng0.png)

### 4.9 整体效果预览

再确认一下整体结构，是否和下图一致，注意各节点之间的连接关系：

![](https://www.bzfree.com/upload/images/coze/kh73jdmBRCQmgBOjvQaBFdoUOAoiJEvEg1rRZUimjhw.png)

细节图一：

![](https://www.bzfree.com/upload/images/coze/QIOblTOPqaR00EmRgsE7wD9C0b9rRFmK-9TVcdzLbv8.png)

细节图二：

![](https://www.bzfree.com/upload/images/coze/M163s1pUnq2knnfnRB2t9lM_HGQfoIBsHqg3L_zaIO0.png)

### 4.10 配置各节点参数参数

#### 4.10.1 设置开始节点参数

![](https://www.bzfree.com/upload/images/coze/Hztt3ioV1UMPn4aEx6VWlJkawMPQ4K6CVx9hzX44Ofs.png)

#### 4.10.2 设置大模型参数

**大模型-操作类型节点** 配置：

1、添加图书 2、删除图书 3、查询列表

![](https://www.bzfree.com/upload/images/coze/D2Vq0zyO61kvSaurCJwAdOn1WcDAdqSeEFWXAzLVxEY.png)

**大模型-提取书名节点** 配置：

![](https://www.bzfree.com/upload/images/coze/zbBrW7MkRaVaMf5ckO4iUqLe6uDifMVeyPHEUHCRPWk.png)

#### 4.10.3 设置选择器参数

选择器-1 配置：

![](https://www.bzfree.com/upload/images/coze/16mIgFuBARP3W2Dm1MQGYhIDBjRY053ULy9u8Bks4mU.png)

选择器-2配置：

![](https://www.bzfree.com/upload/images/coze/Asaog23VBw4TXX_TklxhouTh0Lq0vPC_mWdrBIZ87co.png)

#### 4.10.4 设置数据库参数

数据库添加节点 参数配置

使用自动生成SQL功能生成

![](https://www.bzfree.com/upload/images/coze/TAqa58n8KS3gcFiHpheYhVPiHM8yiYRiFNKs3ENsNoo.png)

修改一下SQL的变量，使用{{book\_name}}

![](https://www.bzfree.com/upload/images/coze/KgdM_XZ6YhIi0_19VsDdO-PPFqw9emZIdeR509WEmds.png)

同样的方法修改 **数据库删除节点** 参数配置。

![](https://www.bzfree.com/upload/images/coze/bJt_ZZP4Y7qRcjBogMwygWkBuIjjI5MZxoZ9HLg9v1Y.png)

同样的方法修改 **数据库查询节点** 参数配置，注意图中所示，两个查询的name字段要对应。

![](https://www.bzfree.com/upload/images/coze/AjpKzjuunKprLJ0xNRHjkLmcf4JPR2_fImi3S_nwz1I.png)

**结束节点参数** 设置

![](https://www.bzfree.com/upload/images/coze/UPU1UniCY1je1bH2IwUadJOCWMKVLRQX2TrOCTqWcKk.png)

![](https://www.bzfree.com/upload/images/coze/_y1OEDxCenrZVD_f1YxTYv97JPIN6eu1R5LXazu0Acw.png)

### 4.11. 调试工作流

#### 4.11.1 添加一本书

到这里，各节点的配置以及连接方式，我们就配置好了。接下来我们调试一下，看看是否符合我们的预期要求。

在工作流中点击试运行，输入：增加一本三国演义。然后选择我们之前创建好的Bot：图书管理助手。点击 运行 按钮。

![](https://www.bzfree.com/upload/images/coze/D1c3G7m6y4ZP7hkTh-AirsmlDpXCmLBY855VAdU8P4s.png)

可以看到，是按照预期走的 **添加** 的流程：

![](https://www.bzfree.com/upload/images/coze/RT32QxNST4iS66xzDb-o7nqfofuBARql_emI1vs6wgA.png)

![](https://www.bzfree.com/upload/images/coze/k1pkV9aX084W1noEIcz8ltxU7K--zBP7RTPrnVl4l_4.png)

再增加一本《围城》

![](https://www.bzfree.com/upload/images/coze/7na9wmV7douPYeg8JdfweeVMCbDRsEyHFvbKNXGd3cE.png)

查看结果：

![](https://www.bzfree.com/upload/images/coze/UVT3qOFKoie_WEf6RmziYKx8FR74mhTKzYzM_NSs_7I.png)

可以看到《围城》已经被成功添加了。

#### 4.11.2 删除一本书

我们把之前的添加的《三国演义》删除。点击 **运行** 按钮。

![](https://www.bzfree.com/upload/images/coze/POwRqqQgpxInW6hCOWTz12imV6k1OXYIYVrQx7RmirE.png)

可以看到，按照预期，《三国演义》被删除了。

![](https://www.bzfree.com/upload/images/coze/uLQIHr4cCYDoDIJxeweeth8bB1JKVvOaJ0NtZh9c16o.png)

到此为止，我们的图书管理工作流就调试完成了。😊

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

### 4.12 引入工作流

接下来把工作流引入到Bot中进行使用

找到我们已经创建好的图书管理助手Bot。

![](https://www.bzfree.com/upload/images/coze/x1_7-0Au4pb9qof2R5N4sH-tHMdTUEMdkXng0WmScO8.png)

点击 **+** 引入工作流

![](https://www.bzfree.com/upload/images/coze/hoqjyIHoF8uicLAKPMA9NgFY7mBKC9T_CnGQ9YkZzc4.png)

选择 WorkFlow\_Books 工作流

![](https://www.bzfree.com/upload/images/coze/SioSUIwTY48t2MgCS-xv1jEWT8SmlU5VzosIG0Yrw5Y.png)

编排 **人设与回复逻辑**

![](https://www.bzfree.com/upload/images/coze/TvKiuAHaKKo607mZbQD9c_z_0oJdn_tPYS7b2XTjXM4.png)

### 4.13 调试BOT

添加一本书：

![](https://www.bzfree.com/upload/images/coze/SDORWssJfxNDlUGNkO86CkzatnI3XSTKjyRpkuzbXr4.png)

提示图书已经成功被添加了。

那么接下来测试一下，图书是否确实加入成功了。

![](https://www.bzfree.com/upload/images/coze/DHKf_CcrR78dpvJVc95k7-VdXnIE0dnkxuk21L4FdT8.png)

可以看到，《三国演义》图书确实成功加放到了数据库中，说明我们的工作流正确无误。

### 4.14 发布BOT

调试好以后，我们接下来就可以把BOT出布出去，让大家来使用了。

自动生成开场白，点击 **确认** 按钮。

![](https://www.bzfree.com/upload/images/coze/kzZW4TxtryOh11mSB6HvaYr0P-UdiwVEiQOSekImm88.png)

选择一下想发布的平台，我这里选择的是发布到扣子商店，然后点击 **发布** 按钮。

![](https://www.bzfree.com/upload/images/coze/EYIWwKGFeWs_qK5gtLgtQt2xf8v_uksnvF_4A3kUCoo.webp)

提示审核中，然后点击 **完成** 按钮，一分钟左右就审核完成了。

![](https://www.bzfree.com/upload/images/coze/rTaGABNUTPZp8rzsfcMIRjd-vfcYD9iSPUfH5CCO1sY.png)

好了，到这里，我们终于把Bot和工作流的全部流程学习完了，希望大家在本文中能有所收获。😊

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

## **第六章：图像流创建及使用**

## 1\. 什么是图像流

图像流是可以让用户能够通过直观的方式，灵活地组合图像工具来处理图像的流程。它将图像处理工具模块化，并通过可视化界面将这些模块组合在一起，形成一个完整的处理流程。用户可以根据需要选择不同的工具模块，并通过拖拽的方式将它们连接起来，形成一个图像处理的“流水线”。每个模块代表一个具体的图像处理功能，如裁剪、调整亮度、添加滤镜等，用户可以随时调整模块的顺序或参数，以达到最佳的处理效果。

**举个例子：创建一个简单的图像处理流**

假设你有一张风景照片，想要通过图像流实现以下处理流程：裁剪图像 -> 调整亮度和对比度 -> 添加滤镜 -> 添加水印。

**裁剪图像：**

拖拽“裁剪”模块到工作区域。

设置裁剪区域的大小和位置。

**调整亮度和对比度：**

拖拽“亮度/对比度调整”模块并连接到“裁剪”模块的输出。

调整亮度和对比度的参数，实时预览结果。

**添加滤镜：**

拖拽“滤镜”模块（如“黑白滤镜”）并连接到“亮度/对比度调整”模块的输出。

选择滤镜类型和强度，实时预览结果。

**添加水印：**

拖拽“水印”模块并连接到“滤镜”模块的输出。

上传水印图像，调整水印的位置和透明度。

\*\*通过图像流的直观界面，用户可以轻松地将这些模块连接在一起，形成一个完整的图像处理流程。\*\*每个模块的参数调整和处理结果都可以实时预览，用户可以随时调整参数或模块顺序，以达到最佳的处理效果。

## 2\. 图像流的组成

如图中所示，图像流是由多个**工具节点**组合而成的一整套流程。\*\*工具节点是组成图像流的基本单元。\*\*例如，智能抠图工具、美颜工具、画质提升工具等。

工作流默认包含了**开始节点**和**结束节点**。

开始节点是图像流的起始节点，可以包含用户输入信息。

结束节点是图像流的末尾节点，用于返回工作流的运行结果。

![](https://www.bzfree.com/upload/images/coze/adwpVSwMZ5hfOnGO4wjVjXdEFURYj5FvltD9mCvqkr0.png)

工具节点分了三个大类：**智能生成**、**智能编辑**和**基础编辑**，接下来我们一一介绍。

## 3\. 工具节点示例详解

### 3.1 文生图工具

文生图工具可以通过文字描述生成图片。

下面我们通过一个示例，来看一下文生图工具的作用。

这个示例是：输入一段文字，生成漫威人物“钢铁侠”。

先看一下文生图工具每个参数的含义：

ratio（宽高比例）：生成图像的宽高比例,支持1(1:1)、2(4:3)、3(16:9)、4(3:4)、5(9:16)

width（图片宽度）：图片宽度,范围为\[576,1728\]，默认为1088，宽\*高不可以超过1088\*1088个像素点。

height（图片高度）：图片高度,范围为\[576,1728\]，默认为1088，宽\*高不可以超过1088\*1088个像素点。

prompt（提示词）：用于生成图像的提示词。

![](https://www.bzfree.com/upload/images/coze/8hTpMWjCOFXpADKtwtojr-T5Eei-8w2EGXgdcgLiQ6w.png)

下面开始案例的实际演示：

把文生图工具节点添加到视图中

![](https://www.bzfree.com/upload/images/coze/yyXiYVFNT-sbL_fjUOBXImGwJaY_jsy9kDF5zNpg0xw.png)

设置文生图工具节点的参数：

宽高比例我这里设置为1:1。大家可以根据自己的需要进行设置，支持1(1:1)、2(4:3)、3(16:9)、4(3:4)、5(9:16)。

宽度和高度我设置的是300。为了演示方便，我没有设置太大的值，这里的值太大会生成速度会有影响，大家根据自己的需要进行设置，建议够用即可。

提示词prompt直接引用开始节点中的用户输入的图像描述指令。

节点参数设置如下：

![](https://www.bzfree.com/upload/images/coze/X_xU8cM8Alr_7ig9uK0BFFzG8GCKIR6VEDuEhMjQmEU.png)

接下来，点击试运行，测试一下效果。

![](https://www.bzfree.com/upload/images/coze/BUCO-WtsGP7sHSEVurDZ1dTSXadJofaPc0G5lny8Ac4.png)

输入图像描述指令：

![](https://www.bzfree.com/upload/images/coze/DPPv9Uv9lY0hHfXuREBOzqjw-_tAvd4ESWvcbXON2TI.png)

运行结果：

![](https://www.bzfree.com/upload/images/coze/eNnfDi4IxuKGBnSfYx5Y6d_9Qtc-jLXf45_fKtAm-2Y.png)

看一下效果，确实是钢铁侠 ，不过这神态有点像刚刚加完班的感觉，😁 ~~

好了，关于文生图工具节点就为大家讲到这里。要想画出更好的效果，就要配合更好的提示词，接下来就看你的了 ~

### 3.2 智能换脸

智能换脸工具可以为图片替换参考图的人脸。

先看一下文生图工具每个参数的含义：

**reference\_picture\_url(参考图)：** 想要替换脸的人物脸照片。可以上传一张图片，也可以输入一个URL地址。

**skin(美肤效果)：** 范围\[0,1\]，越高美肤效果越好。

**template\_picture\_url(模板图)：** 被替换脸的人物照片。可以上传一张图片，也可以输入一个URL地址。

![](https://www.bzfree.com/upload/images/coze/POkARdFIDzv5s3smWwUhK3YZAWYE7yv8T3eL80lJIbU.png)

下面我们通过一个示例，来看一下智能换脸工具的作用。

这个示例的作用是：使用马斯克的脸替换模板图中人物的脸。😁 ~~

把智能换脸工具节点添加到视图中

![](https://www.bzfree.com/upload/images/coze/yyXiYVFNT-sbL_fjUOBXImGwJaY_jsy9kDF5zNpg0xw.png)

设置智能换脸工具节点的参数：

**参考图**这里我上传了一张马斯克图像：

![](https://www.bzfree.com/upload/images/coze/GSXVkJgP4DNP3iAc0_4Sw2QtoKbctlpMemGhVTSp8RQ.jpeg)

**模板图**上传一张想被马斯克的脸替换的人物。（以下人物为AI虚拟生成）

![](https://www.bzfree.com/upload/images/coze/Dds6hBpfAtEh9qROMweVyt3rpydo9DDyiQAp-Uc84kU.png)

美肤效果设置为1。

具体参数设置如下：

![](https://www.bzfree.com/upload/images/coze/KMMayZSjHMXfCx1xIw04q9FlsUGO9twv6V7gFDA8dl0.png)

接下来，点击试运行，测试一下效果。

![](https://www.bzfree.com/upload/images/coze/B8FvpmYhgcl2PrAImClWNZDYURgNVoEnAlDmmvSp69s.png)

输入图像描述指令：

![](https://www.bzfree.com/upload/images/coze/DPPv9Uv9lY0hHfXuREBOzqjw-_tAvd4ESWvcbXON2TI.png)

运行结果：

![](https://www.bzfree.com/upload/images/coze/N4fdDh8w0FW_0_ndTLwiGnSeOtZzvbY49V7KeX3d8hI.png)

看一下效果，就算换一个发型，照样是马斯克，😁 ~~

好了，关于智能换脸工具就为大家讲到这里。要想生成出更好的效果，大家就多多使用不同风格的图片尝试一下吧 ~

### 3.3 背景替换工具

背景替换工具可以为图片替换背景图。

先看一下背景替换工具中每个参数的含义：

**ref\_prompt\_weight（权重）**：仅当 **ref\_image\_url** 和 **ref\_prompt** 同时输入时生效，该参数设定文本和图像引导的权重。ref\_prompt\_weight表示文本的权重，图像引导的权重为1-ref\_prompt\_weight。默认值0.5,取值范围\[0,1\]。

**scene\_type（使用场景）**：当前包含3种场景：

**base\_image\_url（主体图像URL）**：透明背景的主体图像URL。需要为带透明背景的RGBA四通道图像，支持png格式，分辨率长边不超过2048像素。输出图像的分辨率与该输入图相同。 **noise\_level（噪音等级）**：当ref\_image\_url不为空时生效。在图像引导的过程中添加随机变化,数值越大与参考图相似度越低，默认值300，取值范围\[0,999\]。 **ref\_image\_url（引导图URL）**：支持jpg，png，webp等常见格式图像。ref\_image\_url和ref\_prompt至少输入一个。

**ref\_prompt（引导文本提示词）**：支持中英双语，不超过70个单词。ref\_image\_url和ref\_prompt 至少输入一个。

![](https://www.bzfree.com/upload/images/coze/uNlOzFToaWp3rX62PpMgcoYLmWWWryB6xKf8KgnJO2s.png)

下面我们通过一个示例，来演示一下背景替换工具的作用。

这个示例的作用是：使用一张不带背景的红酒图片，为这瓶红酒生成一个背景。

先把智能换脸工具节点添加到视图中

![](https://www.bzfree.com/upload/images/coze/1gwYZg2zYIx56fUjyRrycMqndPojHHfWJgPbid8Emrk.png)

设置背景替换工具节点的参数：

所有参数中 **base\_image\_url（主体图像URL）**是必填的，其它都可以选填。如果想生成出好的效果图片，这些参数都需要配合使用**。**

我们先上传一张红酒的主体图片，我用的是下面这张演示。

注意：要求这张图片要有一个主体，并且背景是透明的，不然生成出来的图片就不稳定了。

![](https://www.bzfree.com/upload/images/coze/GKfXcF__h6H_BY-dPerMr3ZAOH9HgZUUFQLkPVilK_A.png)

只上传这一张图像，我们也是可以生成的了，但为生成好的效果，我又为图片加了一个**ref\_prompt（引导提示词）**。这个提示词越具体越好，这里大家发挥想象力。

我这里写的是：红酒摆在餐桌上，背景是个酒柜。

同时我也为图片加了一个**scene\_type（使用场景）**，这里我用的是\*\*ROOM(家居场景)\*\*。

具体参数设置如下：

![](https://www.bzfree.com/upload/images/coze/zJwNz8KLBjbQDwbnNSsxd5AKl8Hh62WuafSFsf9Aa-A.png)

接下来，点击试运行，测试一下效果。

![](https://www.bzfree.com/upload/images/coze/sRJ5OG5iytzzIeRkYnp4scrZP3cv8uw_0gMMKAJa06o.png)

运行结果：

![](https://www.bzfree.com/upload/images/coze/yD-o1FljI8S8e93QenFRhWopUB-m-uMapeQivY9u8Kk.png)

看一下效果，效果其实还是可以更好点的，😁 ~~

好了，关于背景替换工具就为大家讲到这里。要想生成出更好的效果，大家就多多搭配其他参数尝试一下吧 ~

### 3.4 多图融合工具

**什么是多图融合：** AI多图融合是一种利用人工智能技术将多张图片结合在一起，生成一张新图片的过程。这种技术可以用于增强图片的视觉效果，提取多张图片中的关键信息，或者创建全新的视觉内容。多图融合技术通常涉及到图像处理、模式识别、机器学习等领域的知识，能够实现多种不同的融合效果，比如通过融合不同视角的图片来创建全景图像，或者将不同风格和内容的图片融合在一起，创造出独特的艺术效果。

**多图融合工具可以为原图添加参考图的风格。**

先看一下多图融合工具中每个参数的含义：

**prompt（提示词）**：对于风格迁移的提示词描述。

**prompt\_strength（提示词影响程度）**：提示词的影响程度，范围(0.1)，越低受提示词的影响程度越高。

**ratio（图像比例）**:目前支持，1=1:1(正方形):1024x1024；2=4:3(横向):1024x768；3=3:4(纵向):768x1024; 4=16:9(宽屏):1024x576；5=9:16(竖屏):576x1024。 \*\*strength\_image1（风格影响程度）\*\*：风格参考图的影响程度，范围(0,1\]。

**strength\_image1（原图影响程度）**：原图的影响程度，范围(0,1\]。 **style（图像风格）**：生成图片的风格。0：人像写实风格；1：动漫风格，默认为0。

**image1**：风格参考图。

**image2**：原图。

![](https://www.bzfree.com/upload/images/coze/HnrZnCvplrFNjvIH8zqjaWxns7zXQQU5LIoLIWMVk8o.png)

下面我们通过一个示例，来演示一下**多图融合工具**的作用。

**这个示例的作用是：把原图的动漫图片转换人像写实风格，并把原图中的人物，融合到参考图的场景中。**

先把多图融合工具节点添加到视图中：

![](https://www.bzfree.com/upload/images/coze/muN7D8ZDuJLxluCMUL24tyalqwik0QweozKpvW0QSyI.png)

设置多图融合工具节点的参数：

其中**原图**和风格**参考图**是必填的，其它都可以选填。如果想生成出好的效果图片，这些参数都需要配合使用\*\*。\*\*

那么，我们就先上传一张原图和一张风格参考图，我用的分别是下面这两张动漫图片演示。

原图：

![](https://www.bzfree.com/upload/images/coze/-N3CvGEUQug6XtJfmEMD0tzsaC6hswp5DGe3RCt03B4.png)

风格参考图：

![](https://www.bzfree.com/upload/images/coze/WeurrL0ZZlych-7q5nkeTU6tmSzU3nmJ6aJYe2aPgXo.png)

因为我们的目的是把原图的动漫图片转换人像写实风格，所以要把**style**参数设置为：0。

具体参数设置如下：

![](https://www.bzfree.com/upload/images/coze/waOBP20zVEqrI6VEoKJMok7N3CdS5qHmJ_KV9aednsA.png)

接下来，测试一下多图融合工具节点。

![](https://www.bzfree.com/upload/images/coze/soiJpz2l7UAJTtnrZCXnAn0EKFkjZVDHWhvHC7O0Lhw.png)

运行结果：

![](https://www.bzfree.com/upload/images/coze/YGypPs85iqe0FhKBBSBgkmS0IBCOWoe9M08b61s0L0U.png)

生成图片：

![](https://www.bzfree.com/upload/images/coze/aDS4ad4tOZ0KKUCqRPPO2V-3z8DfxMXXTlrNT9wFwg0.png)

看一下细节效果，可以看出动漫人物已被转为人像写实风格。从图片中的火焰可以看出，火焰是风格参考图中的特征，说明人物的确已经和参考图中的特征进行了融合。怎么样，效果还不错吧 😊 ~~

好了，关于多图融合工具就为大家讲到这里。要想生成出更好的效果，大家就多多搭配其他参数尝试一下吧 ~

### 3.5 人像风格化工具

**什么是人像风格化：** AI人像风格化是指使用人工智能技术对人物肖像进行艺术化处理，使其呈现出特定的风格或效果。人像风格化能够学习并模仿不同的艺术风格，然后将这些风格应用到人像图片上。

AI人像风格化可以实现多种效果，扣子目前提供的有五种风格模式，分别为：**日漫新海诚**、**水彩风**、**穆夏风**、**2.5D** 和 **水墨风**。

**先看一下人像风格化工具中每个参数的含义：**

**height（图片高）**：目标图高，取值范围为\[1080，1920\]，默认为1536。

**width（图片宽）**：目标图宽，取值范围为\[540，1080\]，默认为864。

**style\_prompt（风格模式）**：

**url**：参考图链接，也就是期望被转换的图。

**user\_prompt（用户提示词）**：用于生成图像的用户提示词。

![](https://www.bzfree.com/upload/images/coze/z32MRC90-7px8av7GvDZgX3FUtruHxqF5eG82AOR8os.png)

下面我们通过一个示例，来演示一下**人像风格化工具**的作用。

**这个示例的作用是：把原图的动漫图片转换为水墨风。**

先把人像风格化工具节点添加到视图中：

![](https://www.bzfree.com/upload/images/coze/weLTxBQHWOxxzfkTmHxAbX7IxFmgKSJg4EuDNSowzmY.png)

设置人像风格化工具节点的参数：

其中**参考图链接**是必填的，其它都可以选填。如果想生成出好的效果图片，这些参数都需要配合使用\*\*。\*\*

那么，我们就先上传一张参考图，我用的是下面这动漫图片演示。

参考图：

![](https://www.bzfree.com/upload/images/coze/-N3CvGEUQug6XtJfmEMD0tzsaC6hswp5DGe3RCt03B4.png)

因为我们的目的是把原图的动漫图片转换水墨风，所以要把**style\_prompt**参数设置为：4。

具体参数设置如下：

![](https://www.bzfree.com/upload/images/coze/EoFdmX_9vZVsC7ZlRzS187b-lhX7PDHEpum7hTA6amU.png)

接下来，测试一下人像风格化工具节点。

![](https://www.bzfree.com/upload/images/coze/SkLab52u73D12g7eeLK1xvN3KsSrHhXVqi288ta54eA.png)

运行结果：

![](https://www.bzfree.com/upload/images/coze/ouggYpx5miJWAnzW-GNGWdtW4e4BK2G0_Ik4oz5MLAU.png)

生成图片：

![](https://www.bzfree.com/upload/images/coze/ZgQ9yrU-ROqu4NW269Ljw_lF5eVX7hjHRxmwdzDXeMs.png)

看一下细节效果，已经完全转换为水墨风格了。效果还不错吧 😊~~

好了，关于人像风格化工具的介绍就到这里。要想生成更好的效果，大家可以多多尝试搭配其他参数哦 ~

### 3.6 新版图像生成

写到这章，刚好赶上扣子的图像流改版升级。这次改版对左侧的功能菜单做了一些合并整合。

例如下图，把模型都整合到一个节点上了。升级以后，界面更清晰了。写好提示词，只需要选择我们想要的风格就可以了。

![](https://www.bzfree.com/upload/images/coze/Q6-9hQoTm50LXcU8Zn247_YmwJQU1GW9st8k0NnSVOU.png)

本节课，我们找一个模型风格测试一下。平时有很多同学想找logo生成的工具，那我们这次试一下这个LOGO设计的工具怎么样。

把图像生成工具节点加入画布。

![](https://www.bzfree.com/upload/images/coze/0GSJkJfr3P4OghGjGTXcQktTmrXpHTGVaEtUmga2bm4.png)

对比改版之前，这里参的参数少了很多，我们只需要改出一个提示词就可以了。

接下来说一下生成LOGO关键词这里。有的同学之前也用过一些其他的LOGO生成工具，大多数人反应效果不是很好。因为图像生成本身对提示词的要求是很高的，模糊的提示词和精准的提示词差距很大的。所以要生成一个好的LOGO，要把关键词分解并细化，这里需要花一些时间对自己的需求仔细琢磨一下。

在这里给大家给大家几点建议，例如你的公司是一个奶制品公司，如果你的提示词这样写：生成一个奶制品公司的LOGO，显然这个提示词太模糊了，效果肯定不会太好，我们先来看一下这个提示词生成的效果：

![](https://www.bzfree.com/upload/images/coze/buaXmIAJuf9XCg1vk2wCraczORM6LyyVdW5eUdanaiU.png)

这个LOGO看起来是一个奶制品公司的LOGO，但还是有些简单。

那如何才能生成效果好的的LOGO呢？那我们就要细化提示词，从以下几个方面：

**品牌名称，品牌故事，起源，理念，工艺，产品，社区，愿景。**

从这几个维度，就能让生成的LOGO立体起来了。

例如，根据上面几点，我用GPT帮我生成了如下提示词，我们用这段提示词测试一下效果：

来看一下效果：

![](https://www.bzfree.com/upload/images/coze/HgD_FAdj1AcqNcOZ1D0YTCydYKuKyE1Xral43iJp5VM.png)

怎么样，是不是效果好了很多。虽然元素丰富了一些，但是感觉色调还是有些单调。这个时我们再借助一下风格工具。

我们把风格滤镜工具节点放入到画布中，然后和前一个节点相连接。

![](https://www.bzfree.com/upload/images/coze/9ChcNHbo-U647A3UaXemJEhmFsVMt2LcJ6G-NNJMLA4.png)

把上一个生成的图像做一个风格的转换。

image\_url对应的是前置节点生成的原始图片，style对应的转换的风格。

风格滤镜目前有6种风格：0为毛毡风、1为粘土风、2为积木风、3为美漫风、4为玉石风、5为搞笑涂鸦风格。

这里我们设置为3，是转换为美漫风格的。

运行看一下效果：

![](https://www.bzfree.com/upload/images/coze/-AJX0xBfc7J3y6EXmjnJhj3mvf-b5jC65KA0jjmYAvI.png)

怎么样，是不是画面丰富了许多。那如果我们用这个图片再做一下简单的编辑，那应该就可以使用了。

当然，我这里只是给大家提供一个思路，大家可以发散思维，多多尝试一些其他的工具节点及风格，相信大家可以创作出更好的LOGO。

好了，今天的讲解就到这里，大家快动手尝试一下把~ 😊

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

\---

### 3.7 图质提升

**最近，有同学在问，有没有一种技术，可以把不清晰的图片变得清晰呢？答案当然是可以的。今天和大家分享一个扣子平台的功能，简单且实用。**

要想把模糊的图片变清晰，这里我们要涉及一种图像处理技术：**图像超分辨率**（Super-Resolution, SR），也就是所谓的**超分**。这是利用图像中的信息和先验知识，推测和还原图像中丢失的细节，从而增加图像的清晰度和细节级别。

**简单理解，就是把低分辨率的图片丢失的部分进行补充，变成高分辨率。**

那扣子中有没有这种工具呢？答案当然也是有的。本节课就为大家讲解扣子图像流中的\*\*「画质提升」\*\*节点。

#### 3.7.1 创建图像流

新建一个图像流：

![](https://www.bzfree.com/upload/images/coze/ebeb0aefded52008edd7ea20105b4924.png)

填写图像流名称：

![](https://www.bzfree.com/upload/images/coze/2ef34aa01c942185ec42ceda98d4288b.png)

把「画质提升」工具节点加入画中：

![](https://www.bzfree.com/upload/images/coze/3ca9e2c2e022605bf5625ada71ab6b44.png)

画质提示节点使用非常简单，连提示词都不需要写。：）

只需上传一张图片即可：

![](https://www.bzfree.com/upload/images/coze/b70b3c644107df536880e78ee73302ab.png)

#### 3.7.2 测试图像流

首先，我们找一张模糊的图片用来测试，先找一张物体的：

![](https://www.bzfree.com/upload/images/coze/9ac0423abe05a731b8d0633c3c108902.png)

这张图片看起来很模糊，行人和汽车都很不清晰。

我们试着运行一下这个图像流：

![](https://www.bzfree.com/upload/images/coze/55f92ffeca3bd5d75838745d8a6faa9c.png)

上传模糊图片：

![](https://www.bzfree.com/upload/images/coze/58ac30b0a65f09c3cbdea3d15951d604.png)

运行后看一下输出的图片效果：

![](https://www.bzfree.com/upload/images/coze/4fda428ae36899716f5d648a8b3dbd05.png)

是不是瞬间变得很清晰了呢?人物和车辆都做了丢失细节的还原。

我们再来测试一张人物照片：

![](https://www.bzfree.com/upload/images/coze/506785ab24f669bd4eccb30d1b86713a.png)

我们来试运行一下，秒变高清大美女

![](https://www.bzfree.com/upload/images/coze/600ff2612de47fb07739991771307f9d.png)

方法很简单，但是不是很实用~ 如果你有一些老旧的照片，或不清楚的图片，都可以用这个试一下，让你的图片秒变清晰哦！~

好了，今天的讲解就到这里，大家快动手尝试一下把 ~

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

___

### 3.8 智能扩图

**今天和大家分享一个扣子图像流中的「智能扩图」工具节点，这个节点的作用是：可以在扩大图片的同时，并自动生成图像缺失的部分。**

#### 3.8.1 示例对比

我们来用两组图片做一下对比，看看 **「智能扩图」** 的神奇之处。

先对比一组3：4比例的图片。左侧是原图，右侧是使用智能扩图生成的。

生成的这张图片扩充了两旁的树木：

![](https://www.bzfree.com/upload/images/coze/6512d0c607dcb398b7413a120691f4b6.png)

再看一组4：3的图像。上面的原图，下面的是生成的。

从下面的图片可以看出，扩充了整个车身，把车窗和后视镜都补充出来了。

![](https://www.bzfree.com/upload/images/coze/7a5892e4871f33500a51a123597ba66c.png)

怎么样，是不是很神奇！~

那接下来我们就来学习一下，如何使用 **「智能扩图」**。

#### 3.8.2 新建图像流

新建一个图像流：

![](https://www.bzfree.com/upload/images/coze/829853e0933c4f450eeb781f64379721.png)

填写图像流名称：

![](https://www.bzfree.com/upload/images/coze/e445bc38aa3d43aed34805b3dc09226a.png)

把 **「智能扩图」** 工具节点加入画布中：

![](https://www.bzfree.com/upload/images/coze/3ba497dfb4c3b7b87a87e282e5e5f64b.png)

接下来，我们来看一下\*\*「智能扩图」\*\*每个参数的含义：

**url：** 原图链接。

**left（向左扩展比例）：** 范围为（0,1\]，举个例子：原图的宽是100像素，希望扩展到110像素。那就是增加了10%，所以比例应该是0.1。

**right（向右扩展比例）：** 范围为（0,1\]，同上。

**top（向上扩展比例）：** 范围为（0,1\]，举个例子：原图的高是100像素，希望扩展到110像素。那就是增加了10%，所以比例应该是0.1。

**bottom（向下扩展比例）：** 范围为（0,1\]，同上。

**custom\_prompt（提示词）：可以给出需要扩展部分的提示词，这里根据需要填写，也可以默认不填。**

#### 3.8.3 测试图像流

接下来进行测试，先上传一张图片：

![](https://www.bzfree.com/upload/images/coze/756bab1b6ff121e9637cad5fa76267ef.png)

原图为：

![](https://www.bzfree.com/upload/images/coze/0bc779eca55b0ab6adbda95aaacf8acd.png)

然后设置扩充比例，我们的需求是把这张图片左边和右边分别扩充50%。

那么参数分别应该为：left：0.5，right：0.5。

如图所示：

![](https://www.bzfree.com/upload/images/coze/6f6216bde286fe38d3c24caa49000154.png)

我们试着运行一下这个图像流：

![](https://www.bzfree.com/upload/images/coze/35bd8854daf3c4e9282feed71fda6340.png)

运行后看一下输出的图片效果：

![](https://www.bzfree.com/upload/images/coze/7457226f5e3da97d31b55a3354b9551e.png)

怎么样，效果是不是很不错，毫无违和感 ~

#### 3.8.4 应用场景

**「智能扩图」** 一般的应用场景是：

例如：在电商网站首页制作横幅时，想使用一个好看的图片，尺寸比例却达不要求，不是拉伸了，就是压扁了 ，那就可以试试这种方法了。

例如：你想为你的博客或自媒体文章配图，图片比例不对，也可以用 **「智能扩图」** 来制作。

好了，今天的讲解就到这里，大家快动手尝试一下把，可以应用到很多地方噢 ~

🐎 正在快马加鞭准备中，先关注公众号，会及时收到更新通知 ~ 💨

___

关注公众号

![斜杠君微信公众号二维码](https://www.bzfree.com/upload/images/common/qrcode.jpg)

进群交流

![](https://www.bzfree.com/upload/images/common/qrcode-1-gnri.png)

**如果有任何疑问，欢迎进群交流讨论。**

___

## 第七章：卡片的制作及使用

## 1\. 什么是卡片

扣子平台中的「卡片」简单说就是让输出的格式更好看。例如你在扣子上通过插件或工作流返回一篇新闻，如果直接输出，就是一行标题，一段内容，可能有的还会有一个链接。但如果在大模型输出之前，你把这些信息按设定好的格式做成一个好看的卡片，是不是更能提供应用的用户体验，例如下面这样：

![](https://www.bzfree.com/upload/images/coze/rq1qpbU5U1GUJ3Z_eCN728by_ZajvWJE9loiXVtljic.png)

当然，也可以有列表形式的卡片：

![](https://www.bzfree.com/upload/images/coze/uZHsub7VBu66ychpIWG9OTCpVxFAYpTw7_curV7DgsE.png)

## 2\. 卡片的组成

组成卡片的元素叫做组件。

组件一共分两种：

1.  布局组件
2.  基础组件

**布局组件**就是用来划分整体区域的，布局组件有如下几种：

![](https://www.bzfree.com/upload/images/coze/7_qFMsTz5OrIUNlsfttqT_eOm4hezEGuC5ZnZ2MaETk.png)

对于每一个布局，都可单独进行参数的设置，这样就能组合出很多不同的布局。

例如这个布局，

![](https://www.bzfree.com/upload/images/coze/oxO3w0DA9L1ZYE6rc3iddb8YMdPlGKbbMKydctRp_y0.png)

原始的每行展示数目是3个，我可以改成4个，就变成这样了。

![](https://www.bzfree.com/upload/images/coze/D-kiCxF5TmAN89_sN-lgHyVaFMrxQnNfyASkVJEAK_8.png)

**基础组件**是具体的展示信息的类型，例如是图片，还是文本，还是按钮等。

基础组件有如下几种：

![](https://www.bzfree.com/upload/images/coze/RXPSi83IoGr_AjJ-UHuYezryXqfcmGLbzjh5X1K9Bko.png)

如下这个卡片就由一个图片和两个文本元素组成。

![](https://www.bzfree.com/upload/images/coze/K5MVQsxXLsZl_CsEC1rudzuC5EAvCWvSFFr-bRfWHHE.png)

接下来让我们动手制作一个卡片，然后再使用这个制作好的卡片。通过本节课学习，彻底让大家掌握扣子卡片的使用，让你的应用与众不同。

## 3\. 卡片使用范围

-   目前消息卡片仅在豆包客户端、飞书客户端内生效。
-   仅工作流和插件功能支持添加消息卡片。

## 4\. 制作卡片

接下来我们来通过一个实际的案例来学习卡片的制作。

**这个案例的作用是：调用知乎热榜插件，然后用卡片列表的形式展示给用户。**

### 1\. 设置布局

形式如下图所示：

暂时无法在飞书文档外展示此内容

我们要做上面这种类型的卡片，首先要对内容进行分解。从图中可以看出这是一个新闻列表的循环。

所以首先要做出一条新闻的样式，再通过循环就可以展示出多条新闻的列表形式了。

也就是先做出这部分：

![](https://www.bzfree.com/upload/images/coze/47GB5Le2-1qpwjsyKb0JB0Jitl6JOExIfQZjp0NGDVw.png)

上面的这个结构，可以看出，是一个两列布局，有左右两部分内容。左侧是图片，右侧是信息。

那我们首先在画布上添加二列布局组件：

![](https://www.bzfree.com/upload/images/coze/uDX0dX6qhdHJdh8FawY2K700R_9PAGPmvmVD3fSuKV8.png)

然后在这个布局里加入一个图片组件：

![](https://www.bzfree.com/upload/images/coze/aezlSSmZlkUj8rOQbFFrlKixZknDu-U9KJEQlC_DZm4.png)

因为我们想要的图片是正方形，这么布局的话，比例不对。应该把1的宽度变小。

![](https://www.bzfree.com/upload/images/coze/jp1_LEZ1n49wYHGcCeT_pKv8ibZ2ZqXWDH8bw7ygWsg.png)

例如下图这样，把这个宽度再多分几份，实际是6份：

![](https://www.bzfree.com/upload/images/coze/v02MOimM1pZhVNl1UfaZk2enF_EJOPNBiGF-Jrb01Hw.png)

这时让图片的部分占1分，让文字的内容占5份，这样就能达到我们的效果了。

那该应该如何设置呢？

只需要调整信息部分宽度比例即可，改为5：

![](https://www.bzfree.com/upload/images/coze/tVg5M_rEMbeIAgPg57P1qp2WMxYthyMX5trUuyvbCiE.png)

这样比例就调整好了。

### 2\. 添加组件

先添加图片组件：

![](https://www.bzfree.com/upload/images/coze/O44AXRK9SIqGoG_NPngjFjL6n6FWHKMs2BADdXTfmFM.png)

再添加文本组件。文字部分有上下两行，一行是标题，给行是摘要。

那么我们需要添加两个文本组件。

![](https://www.bzfree.com/upload/images/coze/ANXyrLoLu56YuZoi40Qb2vbdh-FcYFOMCC_Avtyi9Og.png)

这样结构就准备好了。通过点击结构的按钮，可以看到当前卡片的结构。如下图：

![](https://www.bzfree.com/upload/images/coze/AF0Xx08aBsAQJfM-xrSJ9gTW_WtuJFGQTu2W025aMJ4.png)

### 3\. 新建变量

因为列表是循环的展示的。正常情况下，循环的数据是接口返回的。在我们这个例子中，就是知乎返回的一个热榜数组。所以在没有调用接口之前，我们需要先通过模拟一个数组来展示这循环列表。

通过变量选项卡新建一个变量：

![](https://www.bzfree.com/upload/images/coze/NfNaFomoOmGxaER5VWbB21Ohm0D3weiu8qnrVjNjIho.png)

这里要注意，如下图所示，变量类型要选择数组：

![](https://www.bzfree.com/upload/images/coze/6A1FWrgTIUAP99h1ibRgvOw4jcpSc5owQCrBhWFqKj8.png)

数组变量的值如下，一共有三个元素，也就是对应展示出来的新闻列表也应是三条。

大家可以复制以下数组使用：

设置好以后，接下来我们为卡片元素绑定变量。

### 4\. 绑定变量

选中最外层组件，打开右侧高级配置中的循环渲染开关。如下图：

![](https://www.bzfree.com/upload/images/coze/FMgqqMGCjs_D3j5AGNxg1kR_SeABYJmZ_AWxYL7jds8.png)

选择刚才我们创建的列表变量：

![](https://www.bzfree.com/upload/images/coze/9sO7SrNBd-11U0q9GpOLX9YwlU71STArz2T58j4IiyU.png)

可以看到，列表循环展示出来了。循环的数量(三条数据)和我们设置的变量也是一一对应的。

接下来绑定元素（图片、标题、摘要）对应的变量。

图片：

![](https://www.bzfree.com/upload/images/coze/Hh_JfQBLqeZaYtpHBrYTNDiGwHyfdM0cntSLcE8MUzE.png)

标题：

![](https://www.bzfree.com/upload/images/coze/KspR3DVLH3OlX7pT8oC9TOktwROjtAxvz8hTE2d5xEY.png)

摘要：

![](https://www.bzfree.com/upload/images/coze/cvoP4m7lzrc5NrmI33RXX2t_U9qdNDC_y0uKQ6ymXj8.png)

设置好以后是这样的：

![](https://www.bzfree.com/upload/images/coze/wxMMAbfMcVixghu4ofW1vD16Yo3aBx_wj8RnyVSINUk.png)

到这里，我们的卡片制作工作就完成了。接下来让我使用这个卡片小试牛刀~ 😄

### 5\. 保存模板

\*\*注意：这个不是必须的。\*\*但为了下次制作卡片时可以直接引用，一般会保存为模板。

![](https://www.bzfree.com/upload/images/coze/lXZVxjX7EUGg2jS7GE-QxRrzfK6oTQ3xdGvrdN2UX3Q.png)

起一个卡片模板名称：

![](https://www.bzfree.com/upload/images/coze/SD_hFY5naLI0t52rUeLBn-cXqKhCeny8GbUdrULmwo0.png)

### 6\. 发布卡片

**卡片只有发布以后才能被插件或工作流使用。**

点击发布按钮发布一下，如下图：

![](https://www.bzfree.com/upload/images/coze/YC675IzOUETMvY53ApRGGoidMxekip-qcx1y3d98no4.png)

点击确定按钮，就发布好了。

![](https://www.bzfree.com/upload/images/coze/8xVWAq8tn30KytCiPNGbSHZ4MbDU3dWERA-LHa6pfUE.png)

## 5\. 使用卡片

在第三节我们讲过，**工作流和插件功能支持添加消息卡片**。那么我们就通过插件的方式了使用卡片。

注: 如果有同学对插件的使用不了解，可以看第三章的详细教程。

### 5.1 创建Bot

![](https://www.bzfree.com/upload/images/coze/eVbiy73vT7harwg6tc267_sirnL8OooIV4f7wEs98VA.png)

### 5.2 添加插件

因为我们这个例子是要调用知乎热榜的数据，所以这里我们在插件中心搜索知乎热榜插件。

![](https://www.bzfree.com/upload/images/coze/917VEFNhgJCyo33IVSczOYO6oNXwFXcyx0_apO4y1kc.png)

点击添加以后就加好了。

![](https://www.bzfree.com/upload/images/coze/SR7aVZ_GmGH8jG7RqEUEMBtWzgnhKHytbq_tsQm3Fig.png)

### 5.3 配置卡片

点击 **绑定卡片数据按钮** 绑定卡片。

![](https://www.bzfree.com/upload/images/coze/J6QYvpWBQVPD2V-5DOQ_wunXGsKOAxOVAtAAPCa3fE0.png)

选择\*\*「团队卡片」\*\*选项卡，并选择刚才我们发布的卡片。

![](https://www.bzfree.com/upload/images/coze/Vjo7XqUMXrYe_c01LOxk7lVnJDliz6-JigpojttwHM0.png)

绑定数据源。按以下方式，依次绑定插件返回的数据：

![](https://www.bzfree.com/upload/images/coze/u-7V7n0rXg_h-UfePHqRbQGfkcOb3yy0itA565GPSok.png)

绑定之后的数据如下图所示：

![](https://www.bzfree.com/upload/images/coze/8RjN_zu5SWa8hn0A21e00xz2JEjE5tpitu2pvB8s568.png)

### 5.4 测试卡片

卡片设置好了，接下来让我们测试一下吧。

输入查询知乎热榜：

![](https://www.bzfree.com/upload/images/coze/qixiQ-sbmgtphYttk4kFIFUIfrXqjfZlKDgJLl810xI.png)

可以看到，消息以卡片的形式展现出来了。

好了，到这里，我们就把卡片的制作及使用学习完了，希望大家多多使用卡片的形式展现更好的的效果。愿大家在本文中能有所收获。😊