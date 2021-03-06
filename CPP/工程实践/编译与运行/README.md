# 编译与运行

# 编译器对比

GNU(Gnu's Not Unix)编译器套装(GNU Compiler Collection，GCC)，指一套编程语言编译器，以 GPL 及 LGPL 许可证所发行的自由软件，也是 GNU 项目的关键部分，也是 GNU 工具链的主要组成部分之一。GCC(特别是其中的 C 语言编译器)也常被认为是跨平台编译器的事实标准。1985 年由理查德·马修·斯托曼开始发展，现在由自由软件基金会负责维护工作。GCC 原本用 C 开发，后来因为 LLVM、Clang 的崛起，它更快地将开发语言转换为 C++。GCC 在发布后很快地得到扩展，变得可处理 C++。之后也变得可处理 Fortran、Pascal、Objective-C、Java、Ada，Go 与其他语言。

许多操作系统，包括许多类 Unix 系统，如 Linux 及 BSD 家族都采用 GCC 作为标准编译器。苹果电脑预装的 Mac OS X 操作系统也采用这个编译器。GCC 目前由世界各地不同的数个程序员小组维护。它是移植到最多中央处理器架构以及最多操作系统的编译器。由于 GCC 已成为 GNU 系统的官方编译器(包括 GNU/Linux 家族)，它也成为编译与创建其他操作系统的主要编译器，包括 BSD 家族、Mac OS X、NeXTSTEP 与 BeOS。GCC 通常是跨平台软件的编译器首选。有别于一般局限于特定系统与运行环境的编译器，GCC 在所有平台上都使用同一个前端处理程序，产生一样的中介码，因此此中介码在各个其他平台上使用 GCC 编译，有很大的机会可得到正确无误的输出程序。

Clang：是一个 C、C++、Objective-C 和 Objective-C++编程语言的编译器前端。它采用了底层虚拟机(LLVM)作为其后端。它的目标是提供一个 GNU 编译器套装(GCC)的替代品。作者是克里斯·拉特纳(Chris Lattner)，在苹果公司的赞助支持下进行开发，而源代码授权是使用类 BSD 的伊利诺伊大学厄巴纳-香槟分校开源码许可。Clang 主要由 C++编写。Clang 项目包括 Clang 前端和 Clang 静态分析器等。这个软件项目在 2005 年由苹果电脑发起，是 LLVM(Low Level Virtual Machine)编译器工具集的前端(front-end)，目的是输出代码对应的抽象语法树(Abstract Syntax Tree, AST)，并将代码编译成 LLVM Bitcode。接着在后端(back-end)使用 LLVM 编译成平台相关的机器语言。Clang 本身性能优异，其生成的 AST 所耗用掉的内存仅仅是 GCC 的 20%左右。2014 年 1 月发行的 FreeBSD10.0 版将 Clang/LLVM 作为默认编译器。

- GCC 特性：除支持 C/C++/ Objective-C/Objective-C++语言外，还是支持 Java/Ada/Fortran/Go 等；当前的 Clang 的 C++支持落后于 GCC；支持更多平台；更流行，广泛使用，支持完备。

- Clang 特性：编译速度快；内存占用小；兼容 GCC；设计清晰简单、容易理解，易于扩展增强；基于库的模块化设计，易于 IDE 集成；出错提示更友好。
