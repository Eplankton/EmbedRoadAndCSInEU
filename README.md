## 嵌入式软件职业路径与欧陆CS留学工作 —— 理论篇

在国内一说起CS/SE，很多人便产生这样一种幻觉：CS/SE == IT == Web == 互联网大厂，由此产生另一个严重的问题，那就是其他行业，尤其是制造业/工业界的IT现代化水平（以及码农薪资水平）明显落后于互联网行业，形成一个奇特的病态结构。比如嵌入式软件行业，都™的 3202 年了，你却不能在for循环里声明循环变量 i（因为某芯片的编译器只支持C89，上一次更新是2005年），每次看到别人用 Rust 写系统软件时轻快自由的样子，我哗哗地流下羡慕的泪水。造成工具链普遍落后Web 10年甚至20年的原因是大量的嵌入式软件岗位被隔壁电子信息或者自动化或者机械专业转码混过来的人占据，这帮人的代码水平就宛如一个用臭袜子破纸板和胶带缝合在一起做出来的机器人，只能说是“Just Work”（差不多能动就行），无代码测试，无工程交付保证，无法无纪，说不定明天就要爆炸。没有真正学软件的CS/SE人才加入这一行，嵌入式软件就这样一天天地堕落下去没有发展和进步，不发展就没有新鲜血液，就没有高工资，就没有高学历的年轻人，最后搞得校招群里竟然有人灵魂发问：“985的CS爷，不去互联网，来嵌入式干嘛？”。于是整个行业也就这样一天天腐烂下去，好比深圳/东莞血汗电子厂的老板，他们不能理解为什么要为“软件”这种看不见摸不着的东西付费，在他们看来，软件工程师最好免费去给老板打工，还想要工资？滚一边去！老板越是吝啬，越是试图通过降低产品成本来增收并击垮同行，做软件的工资就越低，于是进入一种恶性循环，人力价格不断下降。

新能源汽车的发展，带动汽车电子的发展（请搜索：软件定义汽车），这是嵌软翻身农奴把歌唱的绝佳机会，终于有制造业企业懂嵌入式软件工程师的价值了，要把握这个机会，使得嵌入式软件行业 “脱亚入欧”，变成 CS/SE 行业的一份子，而不是每天在黑乎乎的地下室里接杜邦线盯着示波器，用着1996年来从没更新过的工具软件(注：此软件最高只能兼容 WindowsXP，Win7下必崩溃) 还沾沾自喜。如果你想看看自动化/电气/机械混过来的“嵌入式软件工程师”写代码是什么水平，可以去参观这个回答下面的评论区 [为什么招聘单片机工程师的时候要求精通C/C++? - Qi K的回答 - 知乎](https://www.zhihu.com/question/335790805/answer/2111472871)，然后你就能理解为什么这帮人永远永远永远只能在血汗电子厂里拿着￥3000月薪做消费类电子（还总是想方设法帮老板省硬件成本，殊不知最大的成本™就是从你工资上扣下来的），永远妄自菲薄（自认嵌软比Web低人一等），永远不思进取，永远固步自封。

​本文分成两个主要部分：1.嵌入式软件工程师职业路径 2.欧陆CS留学


## 一、嵌入式软件工程师职业路径

这个嵌入式软件职业规划是完全按照CS/SE(计算机科学/软件工程)专业的培养方案给出的。

https://github.com/m3y54m/Embedded-Engineering-Roadmap 中给出了 RoadMap (此Github 内容持续更新中，里面有相应的资料链接)，我们只参考其中的软件部分，以适合CS/SE的同学，不关心EE(电子信息类)相关的硬件内容。

首先是硬件部分，学校里学过其中一门课程即可：电路原理、数字逻辑(即数电)，还有以下的其中一门：计算机组成原理、计算机体系结构、单片机原理、嵌入式系统原理等。

硬件测试的技能，如逻辑分析仪、万用表等知道怎么用就行，PCB也不需要你来设计，这些都是硬件工程师的工作。

在嵌入式岗位的描述里，“熟悉硬件”、“了解硬件” 这种表述具有丰富的含义，对于大部分嵌入式软件，“熟悉、了解” 这些词的意思为：“知道原理图上某个外设连到什么接口，知道什么是Data Sheet，会查某个外设的寄存器地址和寄存器某个特定的位”，你甚至不用区分电阻和电容，因为都和你无关。越是大企业，你和硬件工程师离的就越远，典型的大企业软件工程师会发现他们的工作流程和互联网码农一模一样：上午写代码、下午写测试用例、下班前合并git repo，甚至还比码农轻松一点，因为少加班。

软件部分是大头，首先，要有熟练的基本编程技能（C/C++/Python）和基本的数据结构与算法知识，学校教的数据结构与算法这样的课程就足够了，嵌入式领域你去刷 LeetCode 没有任何用处（除了面试，不过面试也基本不关心这个）。C/C++的能力是重中之重，熟练吃透C，充分掌握C++（C++11及以上的现代语法越熟练越好，如果你想去高级一点的岗位）以及典型的软件工程设计模型UML之类，汇编能看懂 x86/ARM/RISC-V 中的任意一种即可，没人会让你手搓汇编，看汇编倒是每天要看，Python是用来写构建/测试脚本或者别的一些琐碎代码的，不需要深刻理解，会熟练使用就行。

典型的版本控制工具Git要学会，CMake、GCC等构建工具要熟练、GDB等调试工具要了解。

初入嵌入式编程领域，先使用 Cortex-M 开发板学习最简单的外设：GPIO，然后是经典老三样的通信接口：UART、I2C、SPI，剩下各种外设和传感器跟着野火的教程过一遍即可，非常推荐野火电子的开发板和资料，比如 F1/F4/F7 野火挑战者开发板。



STM32F4 野火开发板学习资料：

[[野火]STM32库开发实战指南——基于野火挑战者开发板 文档 (embedfire.com)](https://doc.embedfire.com/mcu/stm32/f429tiaozhanzhe/std/zh/latest/index.html)

另推荐B站江科大的STM32系列视频：

[【STM32入门教程-2023持续更新中】](https://www.bilibili.com/video/BV1th411z7sn/?share_source=copy_web&vd_source=d0f68c2f26c1bc0a302358246933d32d) 



了解基本的嵌入式编程后，进入 RTOS 领域，回忆一下 操作系统 这门课的知识，删减掉虚拟内存和文件系统这两个部分，剩下的就是 RTOS 需要的知识，在FreeRTOS、μCOS 中选择一个跟着野火电子的资料学就行，学完了可以看看开源的 Zephyr 或者 RT-Thread。

FreeRTOS：[[野火\]FreeRTOS 内核实现与应用开发实战—基于STM32 — FreeRTOS内核实现与应用开发实战指南—基于STM32 文档 (embedfire.com)](https://doc.embedfire.com/rtos/freertos/zh/latest/index.html)

μCOS：[[野火\]uCOS-III内核实现与应用开发实战指南—基于STM32 — [野火]uCOS-III内核实现与应用开发实战指南——基于STM32 文档 (embedfire.com)](https://doc.embedfire.com/rtos/ucos/zh/latest/index.html)

国产的 RT-Thread，中文资料详细全面，适配野火开发板：

[RT-Thread 文档中心](https://www.rt-thread.org/document/site/#/)

[[野火]RT-Thread内核实现与应用开发实战——基于STM32 文档 (embedfire.com)](https://doc.embedfire.com/rtos/rtthread/zh/latest/index.html)



Cortex-M 系列开发板没有MMU，所以不能跑 Linux，如果想学习嵌入式Linux，要换成Cortex-A的开发板，仍然推荐野火/正点原子的开发板，因为资料全面，学习Linux 主要就是学习内核运作的基本原理，如何写bootloader，如何移植内核到开发板上，以及各种外设驱动的编写，外设部分比Cortex-M系列多了MMU，所以有虚拟内存地址映射，其他的没什么不同。

野火IMX开发板学习资料：

[6ULL开发板在线教材与源码仓库 使用Debian 野火鲁班猫镜像 — 野火产品资料下载中心 文档 (embedfire.com)](https://doc.embedfire.com/products/link/zh/latest/linux/ebf_i.mx6ull_doc.html)

[[野火]嵌入式Linux基础与应用开发实战指南——基于i.MX6ULL开发板 文档 (embedfire.com)](https://doc.embedfire.com/linux/imx6/linux_base/zh/latest/index.html)

此外，

对于物联网：买一块乐鑫的ESP32/ESP8266，学习WIFI，MQTT，Zigbee，BLE 这些协议，还需要一些计算机网络方面的知识

对于新能源汽车电子：学习CAN、ModBus，ECU 等工业总线协议，QNX，AUTOSAR等OS


最后，还有一些其他可选的选修课：FPGA、密码学、网络安全、操作系统安全、机器学习、机器人ROS、高性能计算等。

TinyML的例子，适合玩AI/ML/CV炼丹的同学，感兴趣可以看看，256kb RAM 跑ML：https://github.com/mit-han-lab/tiny-training


完成学习后，尝试做1~2个项目(去知乎b站/Github/Gitee搜开源项目)，着重于RTOS/Linux/IoT等软件方面的知识，不要去碰硬件，因为你玩不过EE的人，记住你的特长是软件，也就是说要深耕 RTOS/Linux 这样的领域。

典型案例：MCU+RTOS+LVGL	  ARM+Linux+QT



**如何配置一个舒舒服服写嵌入式代码的环境？**

建议：

1. 所有要用Linux虚拟机的地方，全部使用 WSL2(Ubuntu) + Windows Terminal + VSCode 三剑客组合替代

2. 做项目不可避免地要用 Keil MDK 这种丑陋又弱智的软件，所以按照野火教程配置好 Keil 之后，如果你想呕吐，那么请赶紧用 Embedded IDE这个插件，按照官方教程配置 VSCode + Armclang(ARM Compiler 6) + Embedded IDE + Cortex Debug + OpenOCD 的组合，所有步骤都在文档中写明，不懂的地方去Embedded IDE 的论坛问就行。从此以后编辑、调试一条龙，支持外设SVD查看修改寄存器、支持实时变量刷新(无断点)，尤其对Cortex-M系列支持的完整。

    [插件](https://marketplace.visualstudio.com/items?itemName=CL.eide) 	[论坛](https://discuss.em-ide.com/)	[文档](https://em-ide.com/zh-cn/)

    

    B站搜索：eide，搜出来的视频看几遍跟着操作，不懂就去论坛多问问，作者有空很快会回答你

    B站视频教程：[【VSCode+EIDE开发STM32，支持标准库、HAL库、LL库，可以在VSCode里进行调试，编译以及下载，代码编辑更舒适，环境搭建超简单。】](https://www.bilibili.com/video/BV1nr4y1R7Jb/?share_source=copy_web&vd_source=d0f68c2f26c1bc0a302358246933d32d) 

    

3. 问嵌入式相关的问题 国外StackOverflow，或者Reddit **r/embedded** 这个sub，国内去百度/CSDN/知乎/博客园/简书/B站 碰碰运气，不可全信

    



注意我们找岗位的时候要专注 “**嵌入式软件开发、MCU、Linux、固件、BSP、中间件、驱动、应用、开发、C/C++**” 这样的字眼，应当避免算法岗，因为算法岗一般都是卷王去，不打ACM还想进？而且多为硕士，卷中卷中卷中卷，比老北京鸡肉卷还卷，凡是和算法沾边的就没一个岗位不卷的。

微信公众号：**嵌入式校招菌** 信息汇总，供参考：

24嵌入式秋招信息表（动态更新中）https://docs.qq.com/sheet/DUW5sUUxxZlBKVlBX

垃圾分类项目开源资料（项目）https://pan.baidu.com/s/16xPvAE4nbSRYV3bxrIPcTA 提取码：rw9z

简历模板及pdf资料https://pan.baidu.com/s/1ozrS9tPEywX0JhluV3nl-g 提取码：edwo

网课学习资料：https://pan.baidu.com/s/1DsRKTw-jQxgZzMMEr5lNYg 提取码：js8b

八股文：https://pan.baidu.com/s/1_uh7SpHYyVD1oSLa91Pqcw 提取码：ttn7




## 二、欧陆CS留学工作


其他参考：

  寄托23瑞典（欧陆）群FAQ https://www.kdocs.cn/l/cuSHmNK2KAXO

  知乎收藏夹 https://www.zhihu.com/collection/809098569

国内互联网行业的畸形优势，使得大CS/SE学生的职业选择似乎只剩下一条道路，经典模板：校内刷高绩点、混科研、打比赛、AI炼丹、发paper ---> 背面试八股文，刷Leetcode ---> 卷大厂实习 --->  保研/留学 英 美 澳 港 新 ---> 去美国大厂/回国大厂。又因为美国佬限制大陆留学签证，现在变成英澳港新申请大爆炸，说留学，言必称英澳港新，言必称QS，最后搞出 墨尔本QS17 > 普林斯顿QS18这样的笑话，我的评价是感觉不如墨尔本...QS高，拳打藤校，脚踢清华，鉴定为玩QS玩的。

这里，我们设计一种佛系的发展思路：校内躺平，保持绩点不低于3.2（百分制80/100）即可，偶尔多写写Github项目 ---->  随意选择一个System/Theory相关的方向，继续写项目 ----> 可以选择先在国内工作三四年（工作经验可以增加录取几率，后续当地找工也一般都要求有经验） ---->  申请欧陆CS留学（非AI非CV非ML非算法，总而言之就是System/Theory方向的项目） ----> 当地找工/回国就业。

可选的System/Theory方向：分布式/并行计算系统、高性能计算、数据库、操作系统/安全、编译器、嵌入式实时系统、计算机架构、网络安全、密码学、形式化方法、编程语言

以及各种交叉领域，比如计算生物、计算数学、计算语言、计算医药、人机交互等，越冷门的方向越好，因为根本没有人和你竞争，System方向三年发不了一篇论文是很正常的事情（反观做AI的一年不发三篇文章都不好意思毕业），也契合欧陆CS科研躺平的特点，梦想赚大钱当人上人的不要来卷，左转英美澳港新谢谢。

其实直接去 CSRanking 查就行，学校排名、学校擅长的方向，比QS靠谱十万倍：https://csrankings.org

计算机系统（system）方向的博士毕业后可以去哪些岗位？与AI方向的博士相比是否有差距？ - 知乎 https://www.zhihu.com/question/590829588

非机器学习方向的 CS PhD 有必要读么？ - 知乎 https://www.zhihu.com/question/307580157

欧陆留学基本知识入门：B站 [Marcsims](https://space.bilibili.com/194560 ) 及算法推送的同风格系列视频

欧陆留学，**课程匹配度**为王，课程匹配度决定0/1的区别(不匹配剩下的全完蛋，所以很难转码，只能试试交叉学科)，GPA/动机信/个人简历/科研等决定60~100的区别，而且可操作性很高，可以灵活变通。

ECTS学分转换：240/本科学分=比例因子，如果本科培养计划总共有160学分，那换算因子就是240/160=1.5，所以你的 1学分 = 1.5 ECTS

典型留学找工路径：申请瑞典荷兰丹麦的CS硕士，毕业后德国荷兰找工作，不行回国投秋招，外企普遍有海投通道

**国家**

推荐：

​	瑞典(无GRE，课程难度适中偏低，英语水平高，最适合学习)

​	荷兰(除了TUD TUE，其他无GRE，学习有一定难度，工作机会比瑞典多)

部分推荐：

​	丹麦(无APS/GRE，学费较贵，但DTU发offer狂魔，学习难度平和，工作机会少)

​	德国(CS工作学习不用德语，但是生活上还是得学德语，GRE+APS，地狱级学习难度，工作机会较多，英语水平不如瑞典荷兰，部分州开始收学费)

​	芬兰(无GRE，政策变动，可能要开始收学费，奖学金多，工作机会少)

谨慎考虑：

​	法国（无学费，项目少，申请流程奇特，课程安排奇特）

​	意大利（学费低，但工资低，工作机会少）

​	挪威（学费生活费过高，工作机会少）



欧陆CS项目列表： Global CS  https://global-cs-application.github.io/

欧陆CS职业问题： https://www.reddit.com/r/cscareerquestionsEU/



**个人推荐，因为我们学校是按排名算绩点的，所以GPA极低，选择的都是保底和冲刺的学校，广撒网，最重要的是稳：**

丹麦：

**DTU** 丹麦科技大学

​	CSE  https://www.dtu.dk/english/education/graduate/msc-programmes/computer-science-and-engineering

```
项目要求 https://www.dtu.dk/english/education/graduate/msc-programmes/computer-science-and-engineering/prerequisites
```



**Aarhus** 奥胡斯大学

​	CS 	https://masters.au.dk/computerscience

```
我们希望申请者拥有学士学位，具有基础计算机科学的全面背景。 这应该包括 计算理论 （形式语言和编译、数理逻辑和不可判定性、算法的设计和分析以及数据结构）、 编程 （面向对象编程、函数式编程、软件架构和交互设计）和 系统 （计算机体系结构） 、操作系统、分布式系统、安全性、数据库）。 对于满足这些要求的学生，我们的硕士课程提供多个 专业 ，例如密码学、算法学、编程语言、人机交互以及普适计算和交互。
所有申请人的理学学士学位都将接受评估，入学的课程基础必须反映当代理论和实践。 在对申请人的评估中，重点关注：
    学士学位课程包含计算机科学科目，其程度满足硕士学位课程提供的大多数专业的先决条件。 为了满足所有专业的先决条件，需要满足以下条件：
        20 ECTS 编程，包括面向对象编程、函数式编程和软件架构。
        20 ECTS计算机系统，包括数据库、计算机体系结构、网络、操作系统、分布式系统和安全。
        20 ECTS 理论计算机科学，包括算法和数据结构、逻辑和可计算性、形式语言和编译器、优化和复杂性理论。
        10 ECTS 人机交互和实验系统开发。
    学士学位课程包含数学、概率论和统计学等 20 个 ECTS 基础科目。
```



​	CE	https://masters.au.dk/computer-engineering-msc-in-engineering

```
大学对任何其他技术或科学学士学位课程的评估都重视吸引基础数学、编程、建模和计算机工程方面的资格。 此外，还评估计算机网络、调节技术和数字信号处理的基本资格以及实际和实验计算机工程实验室工作的基本技能。
因此，大学将评估：
    学士学位水平的数学能力，范围至少为 25 ECTS，涵盖主题：微积分、线性代数、概率微积分和统计学，以及离散数学。
    学士学位水平的计算机技术能力，范围至少为 30 ECTS，涵盖编程和建模、算法和数据结构以及计算机体系结构等主题。
    学士学位水平的能力，范围至少为 10 ECTS 学分，涵盖一个或多个主题：计算机网络、监管技术、数字信号处理或机器学习。
```





荷兰：

**VU & UvA** 阿姆斯特丹大学 & 阿姆斯特丹自由大学 联合CS学位（一次性拿两个大学的学位）

​	joint CS  https://vu.nl/en/education/master/computer-science

```
要入读计算机科学硕士课程，需要计算机科学学士学位或密切相关的课程。 一般来说，我们希望以下科目成为您的学士学位课程的一部分：
    编程 算法 计算机系统 计算机网络 软件工程 逻辑

以下任何一门科目都会增加你被录取的机会：
    数据库 自动机 图论 编译器 机器学习或人工智能 数学（线性代数、离散数学、统计学）
```



**Twente** 特温特大学

​    CS 	https://www.utwente.nl/en/education/master/programmes/computer-science/specialisation/software-technology/

```
了解以下主题：
    计算机科学至少 60 个 ECTS 学分，包括：面向对象编程、计算机组织/体系结构、操作系统、计算机网络、数据库、算法和数据结构；
    至少 20 个 ECTS 学分，包括：微积分、离散数学、概率、统计和线性代数； 数学
    至少 15 个 ECTS 学分。 研究项目和研究方法（计算机科学或相关领域） 
```

​    Embed  	https://www.utwente.nl/en/education/master/programmes/embedded-systems/

```
了解以下主题：计算机体系结构/计算机系统、逻辑推理和形式方法、数字电子、操作系统、编程语言（C++ 和其他）、微积分、线性代数、微分方程、信号和系统
科学研究和设计方法的知识和经验 
```



 

瑞典：

瑞典CS英语要求：

-  English 6 即可，瑞典的大部分CS项目都要求这个标准，再高也没用，不会提高你的录取几率

```
IELTS Academic 雅思
- For English 7: an overall mark of 7.0 and no section below 6
- For English 6: an overall mark of 6.5 and no section below 5.5 (大部分CS项目要求这个标准)
- For English 5: an overall mark of 5.5 and no section below 5.0

TOEFL IBT 托福
- For English 7: Score of 20 (scale 0-30) in written test, total score of 100
- For English 6: Score of 20 (scale 0-30) in written test, total score of 90 (大部分CS项目要求这个标准)
- For English 5: Score of 17 (scale 0-30) in written test, total score of 72

Pearson PTE Academic or PTE Academic Online
- For English 7: Score of 68 (writing 61)
- For English 6: Score of 62 (writing 61) (大部分CS项目要求这个标准)
```



**Chalmers** 查尔姆斯理工大学

​	CSN  https://www.chalmers.se/en/education/find-masters-programme/computer-systems-and-networks-msc/

```
主要研究领域的学士学位（或同等学历）：科学、工程或技术

其他先决条件
数学（至少 15 学分，包括微积分（至少 6 学分）和线性代数（至少 6 学分））
计算机工程概论（至少 5 学分）
通用语言编程（至少 7.5 cr.)（例如 C/C++/Java/Haskell 或类似课程）
和以下课程之一（至少 7.5 cr.）：离散数学或数理统计或概率论或算法或数据结构

优选课程经历：
有限自动机理论与形式语言
数学建模与问题解决
函数式编程
面向机器的编程
嵌入式系统开发 
```



​	SE  https://www.chalmers.se/en/education/find-masters-programme/software-engineering-and-technology-msc/

```
主要研究领域的学士学位（或同等学历）：软件工程、计算机科学、计算机工程、自动化

其他先决条件：
数学（至少 12 学分，包括至少 6 学分的离散数学和至少 6 学分的线性代数）
编程（至少 12 学分，其中必须包括至少 6 学分的面向对象编程）
算法和/或数据结构（至少 6 学分）
基础软件工程或软件工程项目（至少 6 学分）

优选课程经历：数理统计 模型驱动软件开发 
```



**UU** 乌普萨拉大学

​	Embed(偏软件的嵌入式项目)    https://www.uu.se/en/admissions/master/selma/program/?pKod=TIS2M

```
20 个数学学分
计算机科学 30 个学分，包括编程和计算机体系结构课程
```



​	CS  https://www.uu.se/en/admissions/master/selma/program/?pInr=DATA&pKod=TDV2M

```
计算机科学 90 学分，包括编程、算法、数据结构、计算机体系结构和操作系统
30 个数学学分
```



**LiU**  林雪平大学

​	CS  https://liu.se/en/education/program/6mics

```
入学要求
    相当于瑞典 Kandidatexamen 的学士学位，主修以下或同等学科领域之一：
    -计算机科学-信息技术-软件工程-计算机工程
    
    计算机相关学科至少 60 个 ECTS 学分，相当于：
    - 编程 - 数据结构 - 数据库- 软件工程- 计算机硬件 - 计算机网络
    
    至少 24 个 ECTS 数学/应用数学和/或与该项目相关的数学应用学分，包括离散数学、线性代数和微积分课程。
    英语对应瑞典高中教育的英语水平（英语6）
```

 

德国：

TUM 	慕尼黑理工大学

RWTH 	亚琛理工大学

...



芬兰：

Helsinki  赫尔辛基大学

​	CS https://www.helsinki.fi/en/degree-programmes/computer-science-masters-programme

Tampere 坦佩雷大学

​	CS  https://www.tuni.fi/en/study-with-us/software-web-cloud-computing-sciences

Oulu 奥卢大学

​	CS https://www.oulu.fi/en/apply/masters-computer-science-and-engineering



保底大学：DTU LiU Twente Umea Oulu Tampere



主要需要准备材料：

1. 课程描述：就是指你上过的**专业必/选修课(不含思政类)**的课程大纲，分门别类，按照学校官网上的要求整理好去找教务处敲章，详情见知乎

    参考 [武汉大学课程描述](https://github.com/BaoBaoDualang/SmallRunningWiki/blob/main/%E6%AC%A7%E6%B4%B2/%E7%95%99%E5%AD%A6/%E6%AD%A6%E5%A4%A7%E8%AF%BE%E7%A8%8B%E6%8F%8F%E8%BF%B0%E6%A8%A1%E6%9D%BF.pdf)


​	**某门课学分不够，可以相关的课来凑**，比如微积分的学分不够，可以用大学物理来凑，能凑一点是一点，反正课程描述是你自己写的，写在学校官网上的要求X个学分只是参考，重要的是你交的课程描述，他是根据课程描述里面的**内容**判断你这门课是不是符合要求的。这也是为什么很多时候没有明确地指出具体的某门课的名字，而是像“数学，编程”这样笼统地要求

1. 成绩单：就是成绩单，英文版，有学校的章，详情见知乎

2. 英语成绩：雅思、托福、PTE(目前仅瑞典/芬兰接受PTE成绩)

其他材料：

1. 毕业证，**条件录取**后，大四毕业补交
2. 护照
3. 动机信：为什么选择这个学校，未来有什么方向，详情知乎
4. 个人简历：学习经历、擅长的科目、做过的科研、发过的论文、参加的比赛、实习经历，详情知乎



个人留学路线规划：

大一大二注意选课时满足课程匹配度，大三上做一些Github项目/实验室项目，大三下考英语，准备课程描述和个人简历(简历也能用来投实习)等资料，大三暑假找实习，大四上申请，大四全学年实习+毕设同步进行。
