#Step-by-step guide to build a local debugging environment for Swift language source code v5.8.1 //手把手搭建Swift语言源码本地调试环境v5.8.1

## Preface //前言
> The first step to start reading a project source code is to make the project compile and run smoothly by yourself. This is especially importent.

开始阅读一份项目源码的第一步，是先让这个项目能够通过你自己编译通过并且顺利跑起来,这一点尤其重要.

>But Swift source code project is relatively complex, and it's not easy to build a debugging environment. Therefore, this is an unavoidable prerequisite for us to understande and learn the underlying principles of Swift.

而Swift源码工程比较复杂，搭建起一个调试环境并不容易.因此这对于我们理解和学习Swift底层的原理可以说是不能绕过的前提.

>After two months of weekend exploration and many pitfalls, I summarized this article with the aim of helping readers reach a locally debuggable state as soon as possible.

笔者经过2个月周末时间的摸索踩了N多坑后总结这篇文章，目的就是帮助读者尽快达到本地可调试的状态.

## Current status of online information //网上资料现状

>At present, there is very little information on this topic that we can find on the internet, and almost all of them have the following problems:

目前我们在网上能搜到的这方面的资料非常少，而且几乎都存在以下几个问题:

> * **Older Swift verisons**: It is certainly not as valuable for us to continue studying very old versions of Swift code as it is to study newer Swift code.

* **Swift版本比较老**：对于我们来说继续研究非常老版本的Swift代码肯定没有去研究比较新的Swift代码有价值.

