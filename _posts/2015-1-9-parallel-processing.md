---
layout: post
title: Parallel Processing Basic Terminology
---

<div dir="ltr" style="text-align: left;" trbidi="on">
<br />
Hey Everyone. So today I was revising my basics in parallel computing. In this post, I will be sharing with you some of the basic terminologies related to parallel processing.<br />
<br />
<br />
<br />
<div class="separator" style="clear: both; text-align: center;">
<a href="http://2.bp.blogspot.com/-aUleTfUbUeg/VQq4Udt7gMI/AAAAAAAACuc/Q1I5tU3mPww/s1600/parallel.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="http://2.bp.blogspot.com/-aUleTfUbUeg/VQq4Udt7gMI/AAAAAAAACuc/Q1I5tU3mPww/s1600/parallel.png" height="225" width="400" /></a></div>
<div class="separator" style="clear: both; text-align: center;">
<br /></div>
<br />
<br />
<span style="color: red;"><b>Parallel Computer</b></span><br />
<br />
It is defined as the multiple processor computer capable of parallel processing<br />
<b><br /></b>
<span style="color: red;"><b>Parallel Processing</b></span><br />
<br />
It is defined as the process of information processing &nbsp;that emphasis the concurrent manipulation of data elements belonging to one or more processors solving a single problem.Parallel processing is the simultaneous use of more than one CPU or processor core to execute a program or multiple computational threads. Ideally, parallel processing makes programs run faster because there are more engines (CPUs or cores) running it.<br />
<b><br /></b>
<span style="color: red;"><b>Super Computer</b></span><br />
<span style="color: red;"><b><br /></b></span>
It is defined as a general purpose computer capable of solving individual problems a an extremely high computational speed compared to other computer built in the same time period.A supercomputer is a computer at the frontline of contemporary processing capacity – which can happen at trillions of floating point operations per second.<br />
<br />
<span style="color: red;"><b>Throughput&nbsp;</b></span><br />
<span style="color: red;"><br /></span>
The throughput of a device is the number of results it produces per unit time.<br />
<br />
<span style="color: red;"><b>Pipelining</b></span><br />
<span style="color: red;"><br /></span>
A pipelined computation is devised into a number of steps called segments or stages. The output of one segment is the input to the next segment which forms the pipe. Pipelining is performed within a CPU.<br />
<br />
<span style="color: red;"><b>SpeedUp</b></span><br />
<span style="color: red;"><br /></span>
The SpeedUp, <b>S(n)</b> is the ratio b/w time needed for the most efficient sequential algorithm (<b>Ts)</b> and that to the time needed to perform the same computations on a machine incorporating pipelining and/or parallelism(<b>Tp</b>)<br />
<br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <b>&nbsp;i.e S(n) = Ts/Tp</b><br />
<b><br /></b>
<b>SpeedUp </b>is also defined as the time required to run a program on a single processor (n=1) to the time required to run the same program on a parallel computer with n identical processors.<br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <b>&nbsp; &nbsp; &nbsp; i.e S(n) = T(1)/T(n)</b><br />
<b><br /></b>
<b style="color: red;">Degree of Parallelism</b><br />
<span style="color: red;"><b><br /></b></span>
It is defined as the total number of processors required to execute a program<br />
<br />
<span style="color: red;"><b>Kinds of Parallelism - Hardware and Software</b></span><br />
<span style="color: red;"><b><br /></b></span>
Hardware parallelism is built into the machine architecture and software parallelism is exploited by the concurrent execution of machine language instructions in a program.<br />
<br />
<b><span style="color: red;">Parallel Run Time T(n)</span></b><br />
<b><span style="color: red;"><br /></span></b>
It is defined as the time required to run a program on a n-processor machine<br />
<br />
<span style="color: red;"><b>Clock Rate &amp; Cycles Per Instruction(CPI)</b></span><br />
<span style="color: red;"><b><br /></b></span>
It is the clock rate that drives the central processing unit (CPU). It has a constant cycle time and is measured in nanoseconds, usually. It is represented by the roman letter tow. Clock Rate is defined as the inverse if this cycle time.<br />
&nbsp; &nbsp; <br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;<b>&nbsp; &nbsp;i.e clock rate = 1/cycle time</b><br />
<b><br /></b>
The program time is decided by the Instruction Count (IC) or the no of machine instruction to be executed in the program.<br />
<br />
<b>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</b><b>CPI( Cycles per Instruction) = CPU Clock cycles for a program/ IC</b><br />
<b><br /></b>
<b>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; CPU time = CPU Clock Cycles for a program / Clock Cycle Time</b><br />
<b><br /></b>
<b>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;CPU Time(T) = IC X CPI X Cycle Time&nbsp;</b><br />
<b><br /></b>
<b><br /></b>
<b><span style="color: red;">MIPS rate</span></b><br />
<b><span style="color: red;"><br /></span></b>
The speed of a processor is usually measured in terms of Million Instructions per second (MIPS). MIPS rare is given by:<br />
<br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<b>MIPS Rate = Instruction Count (IC) / CPU Time(T) &nbsp;X (10^6)</b><br />
<b>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;= &gt;f / CPI X 10^6</b><br />
<b><br /></b>
<b><span style="color: red;">MFLOPS&nbsp;</span></b><br />
<b><span style="color: red;"><br /></span></b>
MFLOPS stands for Millions of Floating point executions per second and is used as a performance measure. MIPS and MFLOPS are not convertible as they measure different ranges of operations. However, Both are used widely to describe the execution rate and floating point capability of a parallel computer.<br />
<br />
<span style="color: red;"><b>Processor (CPU)</b></span><br />
<br />
A central processing unit (CPU) is the electronic circuitry within a computer that carries out the instructions of a computer program by performing the basic arithmetic, logical, control and input/output (I/O) operations specified by the instructions.<br />
<br />
<span style="color: red;"><b>Graphics Processing Unit (GPU)</b></span><br />
<span style="color: red;"><b><br /></b></span>
A graphics processing unit (GPU), also occasionally called visual processing unit (VPU), is a specialized electronic circuit designed to rapidly manipulate and alter memory to accelerate the creation of images in a frame buffer intended for output to a display.<br />
<br />
GPUs are used in embedded systems, mobile phones, personal computers, workstations, and game consoles. Modern GPUs are very efficient at manipulating computer graphics and image processing, and their highly parallel structure makes them more effective than general-purpose CPUs for algorithms where processing of large blocks of data is done in parallel. In a personal computer, a GPU can be present on a video card, or it can be on the motherboard—in certain CPUs—on the CPU die.<br />
<span style="color: red;"><b><br /></b></span>
<span style="color: red;"><b>Multi-Core Processor</b></span><br />
<span style="color: red;"><b><br /></b></span>
A multi-core processor is a single computing component with two or more independent actual central processing units (called "cores"), which are the units that read and execute program instructions.The instructions are ordinary CPU instructions such as add, move data, and branch, but the multiple cores can run multiple instructions at the same time, increasing overall speed for programs amenable to parallel computing.<br />
<br />
<b><span style="color: red;">Coprocessor</span></b><br />
<b><span style="color: red;"><br /></span></b>
A coprocessor is a computer processor used to supplement the functions of the primary processor (the CPU). Operations performed by the coprocessor may be floating point arithmetic, graphics, signal processing, string processing, encryption or I/O Interfacing with peripheral devices. By offloading processor-intensive tasks from the main processor, coprocessors can accelerate system performance.<b style="color: red;">&nbsp;</b><br />
<br />
A coprocessor may not be a general-purpose processor in its own right. Coprocessors cannot fetch instructions from memory, execute program flow control instructions, do input/output operations, manage memory, and so on. The coprocessor requires the host (main) processor to fetch the coprocessor instructions and handle all other operations aside from the coprocessor functions. In some architectures, the coprocessor is a more general-purpose computer, but carries out only a limited range of functions under the close control of a supervisory processor.<br />
<br />
<b><span style="color: red;">Multi-Processing</span></b><br />
<br />
Multiprocessing is the use of two or more central processing units (CPUs) within a single computer system.The term also refers to the ability of a system to support more than one processor and/or the ability to allocate tasks between them. A Multiprocessor is a computer system having two or more processing units (multiple processors) each sharing main memory and peripherals, in order to simultaneously process programs.<br />
<br />
<b><span style="color: red;">Microprocessor&nbsp;</span></b><br />
<b><span style="color: red;"><br /></span></b>
A microprocessor incorporates the functions of a computer's central processing unit (CPU) on a single integrated circuit (IC), or at most a few integrated circuits. All modern CPUs are microprocessors making the micro- prefix redundant. The microprocessor is a multipurpose, programmable device that accepts digital data as input, processes it according to instructions stored in its memory, and provides results as output. It is an example of sequential digital logic, as it has internal memory. Microprocessors operate on numbers and symbols represented in the binary numeral system.The integration of a whole CPU onto a single chip or on a few chips greatly reduced the cost of processing power.<br />
<br />
<br />
<br /></div>

