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