---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a software engineer at [WiseTech Global](https://www.wisetechglobal.com/). I received my M.S. degree in Computer Science from [Capital Normal University](https://eng.cnu.edu.cn/) in 2023, worked on Operating System, and advised by [Weizhen Sun](https://iec.cnu.edu.cn/szdw/zrjs/fjs/97231.htm) and [Yong Xiang](https://www.cs.tsinghua.edu.cn/info/1127/3592.htm). I received my B.S. degree in Computer Science from [Fuzhou University](https://en.fzu.edu.cn/) in 2019. 

I have a strong interest in A.I technology. I want to build up theory and powerful tools to solve real world problems, such as A.I. for science, LLM for software engineering and ML algorithm. I am currently looking for a remote internship in related fields and want to start a Ph.D. in 2024.

Projects
======

Shared scheduler for the coroutines of Rust
------
<img src='/images/overview.png' width="95%">

We make coroutines can be sheduled across processes. 
- Motivation(s): 
  - The coroutines of Rust can perform asynchronous operations effectively, but only be scheduled within separated process. 
  - The threads of OS can be scheduled across processes, but much more costly with context switching than coroutine.
- Goal(s): 
  - Make coroutines to be a system-level shceduling unit (can be scheduled by OS) without thread-like context switching.
- Method(s): 
  - Take into account both performance and function, we use bitmaps to follow priority scheduling within the kernel and processes, which inspired by the O(1) scheduling algorithm of Linux.

[[code]](https://github.com/AmoyCherry/AsyncOS)  [[writing sample]](/files/Writing%20Sample%20(Wenzhi%20Wang).pdf)