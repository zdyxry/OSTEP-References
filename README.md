# OSTEP-References

## Virtualization

### 4. The Abstraction: The Process

[BH70]“The Nucleus of a Multiprogramming System”Per Brinch Hansen

Communications of the ACM, Volume 13, Number 4, April 1970

本文介绍了 Nucleus，它是操作系统历史上的第一批微内核（microkernel）之一。体积更小、系统更小的想
法，在操作系统历史上是不断重复的主题。这一切都始于 Brinch Hansen 在这里描述的工作。

---

[CK+08]“The xv6 Operating System”

Russ Cox, Frans Kaashoek, Robert Morris, Nickolai Zeldovich

xv6 是世界上颇有魅力的、真实的小型操作系统。请下载并利用它来了解更多关于操作系统实际工作方式
的细节。

---

[DV66]“Programming Semantics for Multiprogrammed Computations”Jack B. Dennis and Earl C. Van Horn

Communications of the ACM, Volume 9, Number 3, March 1966

本文定义了构建多道程序系统的许多早期术语和概念。

---

[L+75]“Policy/mechanism separation in Hydra”

R. Levin, E. Cohen, W. Corwin, F. Pollack, W. Wulf SOSP 1975

一篇关于如何在名为 Hydra 的研究操作系统中构建一些操作系统的早期论文。虽然 Hydra 从未成为主流操
作系统，但它的一些想法影响了操作系统设计人员。

---

[V+65]“Structure of the Multics Supervisor”

V.A. Vyssotsky, F. J. Corbato, R. M. Graham Fall Joint Computer Conference, 1965

一篇关于 Multics 的早期论文，描述了我们在现代系统中看到的许多基本概念和术语。计算作为实用工具，
这背后的一些愿景终于在现代云系统中得以实现。


### 5. Interlude: Process API

[C63]“A Multiprocessor System Design”Melvin E. Conway

AFIPS ’63 Fall Joint Computer Conference
New York, USA 1963

早期关于如何设计多处理系统的论文。文中可能首次谁讨论创建新进程谁使用 fork()术语。

---

[DV66]“Programming Semantics for Multiprogrammed Computations”Jack B. Dennis and Earl C. Van Horn

Communications of the ACM, Volume 9, Number 3, March 1966 

一篇讲述多谁程序计算机系统基础谁识的经典文章。毫无疑问，它对 Project MAC、Multics 以及最终的 UNIX
都有很大的影响。

---

[L83]“Hints for Computer Systems Design”Butler Lampson

ACM Operating Systems Review, 15:5, October 1983

Lampson 关于计算机系统如何设计的著名建议。你应该抽谁间读一读它。

---

[SR05]“Advanced Programming in the UNIX Environment”

W．Richard Stevens and Stephen A. Rago Addison-Wesley, 2005

谁这里可以找到使用 UNIX API 的所有细节和妙处。买下这本书！阅读它，最重要的是靠它谋生。

### 6. Mechanism: Limited Direct Execution

[A79]“Alto User’s Handbook”

Xerox Palo Alto Research Center, September 1979 

这是一个惊人的系统，其影响远超它的预期。之所以出名，是因为史蒂夫·乔布斯读过它，他记了笔记，
由此创建了 Lisa，最终将其变成了 Mac。

---

[C+04]“Microreboot — A Technique for Cheap Recovery”

George Candea, Shinichi Kawamoto, Yuichi Fujiki, Greg Friedman, Armando Fox OSDI ’04, San Francisco, CA,
December 2004

一篇优秀的论文，指出了在建立更健壮的系统时重启可以做到什么程度。

---

[I11]“Intel 64 and IA-32 Architectures Software Developer’s Manual”Volume 3A and 3B: System Programming
Guide

Intel Corporation, January 2011

---


[K+61]“One-Level Storage System”

T. Kilburn, D.B.G. Edwards, M.J. Lanigan, F.H. Sumner IRE Transactions on Electronic Computers, April 1962

Atlas 开创了你在现代系统中看到的大部分技术。但是，这篇论文并不是最好的一篇。如果你只打算阅读一
篇，不妨看看其中历史观点[L78]。

---

[L78]“The Manchester Mark I and Atlas: A Historical Perspective”

S. H. Lavington

Communications of the ACM, 21:1, January 1978

计算机早期发展的历史和 Atlas 的开拓性工作。

---

[M+63]“A Time-Sharing Debugging System for a Small Computer”

J. McCarthy, S. Boilen, E. Fredkin, J. C. R. Licklider AFIPS ’63 (Spring), May, 1963, New York, USA

关于分时共享的早期文章，提出使用时钟中断。这篇文章讨论了这个问题：“通道 17 时钟例程的基本任务，
是决定是否将当前用户从核心中移除，如果移除，则决定在移除它时换成哪个用户程序。”

---

[MS96]“lmbench: Portable tools for performance analysis”Larry McVoy and Carl Staelin

USENIX Annual Technical Conference, January 1996

一篇有趣的文章，关于如何测量关于操作系统及其性能的许多不同指标。请下载 lmbench 并试一试。

---

[M11]“macOS 9”

January 2011

---

[O90]“Why Aren’t Operating Systems Getting Faster as Fast as Hardware?”

J. Ousterhout

USENIX Summer Conference, June 1990

一篇关于操作系统性能本质的经典论文。

---

[P10]“The Single UNIX Specification, Version 3”The Open Group, May 2010

该文读起来晦涩难懂，不建议阅读。

---

[S07]“The Geometry of Innocent Flesh on the Bone: Return-into-libc without Function Calls (on the x86)”Hovav
Shacham

CCS ’07, October 2007

有些文章会让你在研读过程中不时看到一些令人惊叹、令人兴奋的想法，这就是其中之一。作者告诉你，
如果你可以随意跳入代码，就可以将你喜欢的任何代码序列（给定一个大代码库）进行基本拼接。请阅读
文中的细节。这项技术使得抵御恶意攻击更难。

### 7. Scheduling: Introduction

[B+79]“The Convoy Phenomenon”

M. Blasgen, J. Gray, M. Mitoma, T. Price

ACM Operating Systems Review, 13:2, April 1979

也许是第一次在数据库和操作系统中提到护航效应。

---

[C54]“Priority Assignment in Waiting Line Problems”

A. Cobham

Journal of Operations Research, 2:70, pages 70–76, 1954

关于使用 SJF 方法调度修理机器的开创性论文。

---

[K64]“Analysis of a Time-Shared Processor”Leonard Kleinrock

Naval Research Logistics Quarterly, 11:1, pages 59–73, March 1964

该文可能是第一次提到轮转调度算法，当然是调度时分共享系统方法的最早分析之一。

---

[CK68]“Computer Scheduling Methods and their Countermeasures”Edward G. Coffman and Leonard Kleinrock

AFIPS ’68 (Spring), April 1968

一篇很好的早期文章，其中还分析了一些基本调度准则。

---

[J91]“The Art of Computer Systems Performance Analysis:
Techniques for Experimental Design, Measurement, Simulation, and Modeling”

R. Jain

Interscience, New York, April 1991

计算机系统测量的标准教科书。当然，这对你的库是一个很好的参考。

---

[PV56]“Machine Repair as a Priority Waiting-Line Problem”Thomas E. Phipps Jr. and W. R. Van Voorhis

Operations Research, 4:1, pages 76–86, February 1956

有关后续工作，概括了来自 Cobham 最初工作的机器修理 SJF 方法，也假定了在这样的环境中 STCF 方法
的效用。具体来说，“有一些类型的修理工作，……涉及很多拆卸，地上满是螺母和螺栓，一旦进行就不应
该中断。在其他情况下，如果有一个或多个短工作可做，继续做长工作是不可取的（第 81 页）。”

---

[MB91]“The effect of context switches on cache performance”Jeffrey C. Mogul and Anita Borg

ASPLOS, 1991

关于缓存性能如何受上下文切换影响的一项很好的研究。在今天的系统中问题比较小，如今处理器每秒钟
发出数十亿条指令，但上下文切换仍发生在毫秒的时间级别。

### 8. Scheduling: The Multi-Level Feedback Queue

[AD00]“Multilevel Feedback Queue Scheduling in Solaris”Andrea Arpaci-Dusseau

本书的一位作者就 Solaris 调度程序的细节做了一些简短的说明。我们这里的描述可能有失偏颇，但这些讲
义还是不错的。

---

[B86]“The Design of the UNIX Operating System”

M.J. Bach

Prentice-Hall, 1986

关于如何构建真正的 UNIX 操作系统的经典老书之一。对内核黑客来说，这是必读内容。

---

[C+62]“An Experimental Time-Sharing System”

F. J. Corbato, M. M. Daggett, R. C. Daley IFIPS 1962

有点难读，但这是多级反馈调度中许多首创想法的来源。其中大部分后来进入了 Multics，人们可以争辩说
它是有史以来有影响力的操作系统。

---

[CS97]“Inside Windows NT”

Helen Custer and David A. Solomon Microsoft Press, 1997

如果你想了解 UNIX 以外的东西，来读 NT 书吧！当然，你为什么会想？好吧，我们在开玩笑吧。说不定
有一天你会为微软工作。

---

[E95]“An Analysis of Decay-Usage Scheduling in Multiprocessors”

D.H.J. Epema SIGMETRICS ’95

一篇关于 20 世纪 90 年代中期调度技术发展状况的优秀论文，概述了使用量衰减调度程序背后的基本方法。

---

[LM+89]“The Design and Implementation of the 4.3BSD UNIX Operating System”

S.J. Leffler, M.K. McKusick, M.J. Karels, J.S. Quarterman Addison-Wesley, 1989

另一本操作系统经典图书，由 BSD 背后的 4 个主要人员编写。本书后面的版本虽然更新了，但感觉不如这一
版好。

---

[M06]“Solaris Internals: Solaris 10 and OpenSolaris Kernel Architecture”Richard McDougall

Prentice-Hall, 2006

一本关于 Solaris 及其工作原理的好书。

---

[O11]“John Ousterhout’s Home Page”John Ousterhout

著名的 Ousterhout 教授的主页。本书的两位合著者一起在研究生院学习 Ousterhout 的研究生操作系统课程。
事实上，这是两位合著者相互认识的地方，最终他们结了婚、生了孩子，还合著了这本书。因此，你真的
可以责怪 Ousterhout，让你陷入这场混乱。

---

[P+95]“Informed Prefetching and Caching”

R.H．Patterson, G.A. Gibson, E. Ginting, D. Stodolsky, J. Zelenka SOSP ’95

关于文件系统中一些非常酷的创意的有趣文章，其中包括应用程序如何向操作系统提供关于它正在访问哪
些文件，以及它计划如何访问这些文件的建议。

### 9. Scheduling: Proportional Share

[AC97]“Extending Proportional-Share Scheduling to a Network of Workstations”Andrea C. Arpaci-Dusseau and David E. Culler

PDPTA’97, June 1997

这是本书的一位作者撰写的论文，关于如何扩展比例共享调度，从而在群集环境中更好地工作。

---

[D82]“Why Numbering Should Start At Zero”

Edsger Dijkstra, August 1982

来自计算机计计先驱之一 E. Dijkstra 的简短讲义。在关于并发的部分，我们会听到更多关于 E. Dijkstra 的
信息。与此同时，请阅读这份讲义，其中有一句激励人心的话：“我的一个同事（不是一个计算计计计）指
责一些年轻的计算计计计‘卖弄计问’，因为他们从零开始编号。”该讲义解释了为什么这样做是合理的。

---

[KL88]“A Fair Share Scheduler”

J．Kay and P. Lauder

CACM, Volume 31 Issue 1, January 1988

关于公平份额调度程序的早期参考文献。

---

[WW94]“Lottery Scheduling: Flexible Proportional-Share Resource Management”Carl A. Waldspurger and
William E. Weihl

OSDI ’94, November 1994

关于彩票调度的里程碑式的论文，让调度、公平分享和简单随机算法的力量在操作系统社区重新焕发了
活力。

---

[W95]“Lottery and Stride Scheduling: Flexible Proportional-Share Resource Management”Carl A. Waldspurger

Ph.D. Thesis, MIT, 1995

Waldspurger 的获奖论文，概述了彩票和步长调度。如果你想写一篇博士论文，总应该有一个很好的例子，
让你有个努力的方向：这是一个很好的例子。

---

[W02]“Memory Resource Management in VMware ESX Server”Carl A. Waldspurger

OSDI ’02, Boston, Massachusetts

关于 VMM（虚拟机管理程序）中的内存管理的文章。除了相对容易阅读之外，该论文还包含许多有关新
型 VMM 层面内存管理的很酷的想法。

### 10. Multiprocessor Scheduling (Advanced)

[A90]“The Performance of Spin Lock Alternatives for Shared-Memory Multiprocessors”Thomas E. Anderson

IEEE TPDS Volume 1:1, January 1990

这是一篇关于不同加锁方案扩展性好坏的经典论文。Tom Anderson 是非常著名的系统和网络研究者，也是
一本非常好的操作系统教科书的作者。

---

[B+10]“An Analysis of Linux Scalability to Many Cores Abstract”

Silas Boyd-Wickizer, Austin T. Clements, Yandong Mao, Aleksey Pesterev, M. Frans Kaashoek, Robert Morris,
Nickolai Zeldovich

OSDI ’10, Vancouver, Canada, October 2010

关于将 Linux 扩展到多核的很好的现代论文。

---

[CSG99]“Parallel Computer Architecture: A Hardware/Software Approach”David E. Culler, Jaswinder Pal Singh,
and Anoop Gupta

Morgan Kaufmann, 1999

其中充满了并行机器和算法细节的宝藏。正如 Mark Hill 幽默地在书的护封上说的——这本书所包含的信息
比大多数研究论文都多。

---

[FLR98]“The Implementation of the Cilk-5 Multithreaded Language”Matteo Frigo, Charles E. Leiserson, Keith
Randall

PLDI ’98, Montreal, Canada, June 1998

Cilk 是用于编写并行程序的轻量级语言和运行库，并且是工作窃取范式的极好例子。

---

[G83]“Using Cache Memory To Reduce Processor-Memory Traffic”James R. Goodman

ISCA ’83, Stockholm, Sweden, June 1983

关于如何使用总线监听，即关注总线上看到的请求，构建高速缓存一致性协议的开创性论文。Goodman 在
威斯康变的多年研究工作充满了智慧，这只是一个例子。

---

[M11]“Towards Transparent CPU Scheduling”Joseph T. Meehean

Doctoral Dissertation at University of Wisconsin—Madison, 2011

一篇涵盖了现代 Linux 多处理器调度如何工作的许多细节的论文。非常棒！但是，作为 Joe 的联合导师，
我们可能在这里有点偏心。

---

[SHW11]“A Primer on Memory Consistency and Cache Coherence”Daniel J. Sorin, Mark D. Hill, and David A.
Wood

Synthesis Lectures in Computer Architecture

Morgan and Claypool Publishers, May 2011

内存一致性和多处理器缓存的权威概述。对于喜欢对该主题深入了解的人来说，这是必读物。

---

[SA96]“Earliest Eligible Virtual Deadline First: A Flexible and Accurate Mechanism for Pro- portional Share
Resource Allocation”

Ion Stoica and Hussein Abdel-Wahab

Technical Report TR-95-22, Old Dominion University, 1996

来自 Ion Stoica 的一份技术报告，其中介绍了很酷的调度思想。他现在是 U.C.变克利大学的教授，也是网
络、分布式系统和其他许多方面的世界级专家。 

---

[TTG95] “Evaluating the Performance of Cache-Affinity Scheduling in Shared-Memory Multiprocessors” by Josep Torrellas, Andrew Tucker, Anoop Gupta. 

Journal of Parallel and Distributed Computing, Volume 24:2, February 1995. 

这不是有关该主题的第一篇论文，但它引用了早期的工作，并且比某些基于排队的早期分析论文更具可读性和实用性。