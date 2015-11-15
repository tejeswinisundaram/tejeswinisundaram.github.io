---
layout: post
title: The Intel Xeon Phi Coprocessor
---

<div dir="ltr" style="text-align: left;" trbidi="on">
<div class="separator" style="clear: both; text-align: center;">
<a href="http://2.bp.blogspot.com/-A1mGAoWVxF4/VLn2cAInDJI/AAAAAAAACKo/bBu_P5FlGoQ/s1600/execution%2Bmodes.png" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><br /></a></div>
Hey Guys.<br />
<br />
As a part of my new assignment, I have begun reading about the all new and powerful Intel Xeon Phi co-processor and its capabilities.<br />
<br />
Here is a brief understanding of the basics.<br />
<br />
<span style="color: red;">1. What is High Performance Computing (HPC) ?&nbsp;</span><br />
<br />
High-performance computing (HPC) is the use of super computers and 
parallel processing techniques for solving complex computational 
problems. High-performance computing evolved due to meet increasing demands 
for processing speed.<br />
<br />
HPC brings together several technologies such as<br />
<ul style="text-align: left;">
<li>computer architecture</li>
<li>&nbsp;algorithms</li>
<li>&nbsp;programs&nbsp;</li>
<li>&nbsp;electronics,&nbsp;</li>
<li>and system 
software&nbsp;</li>
</ul>
under a single canopy to solve advanced problems effectively 
and quickly. HPC systems have the ability to deliver sustained performance through the concurrent use of computing resources.The terms high-performance computing and supercomputing are sometimes used interchangeably. <br />
<br />
<span style="color: red;">2. What is a co-processor?&nbsp;</span><br />
<span style="color: red;"><br /></span>
A coprocessor is a computer processor used to supplement the functions of the primary processor (the CPU). Operations performed by the coprocessor may be floating point arithmetic, graphics, signal processing, string processing, encryption or I/O Interfacing with peripheral devices. By offloading processor-intensive tasks from the main processor, coprocessors can accelerate system performance.<br />
<br />
A coprocessor may not be a general-purpose processor in its own right. Coprocessors cannot fetch instructions from memory, execute program flow control instructions, do input/output operations, manage memory, and so on. The coprocessor requires the host (main) processor to fetch the coprocessor instructions and handle all other operations aside from the coprocessor functions.<br />
<span style="color: red;"><br /></span>
<span style="color: red;">3. What is the Xeon Phi coprocessor?</span><br />
<br />
Intel Xeon Phi coprocessors are PCI Express form factor add-in cards 
that work synergistically with Intel® Xeon® processors to enable 
dramatic performance gains for highly parallel code—up to 1.2 
double-precision teraFLOPS (floating point operations per second) per 
coprocessor.<br />
<br />
Intel Xeon Phi cores are Pentium cores and works as coprocessor to host processor. Due to the fact that it is based on Pentium core allowed developers to port many of the tools and development environment from Intel® Xeon® <br />
based processor to the Xeon Phi coprocessor. The Xeon Phi runs on a Micro OS<br />
based on Linux kernel rather than the driver based model often used for PCI express based attached cards like Graphics cards on a system. <br />
<br />
<span style="color: red;">4. What are the execution models in the Intel Xeon Phi coprocessor?</span><br />
<br />
There are various execution models that can be used to design and execute an application on Intel® Xeon Phi coprocessor in association with the host processor. The programming models supported for the coprocessor may vary <br />
between the Windows OS and Linux OS used on the host system.<br />
<br />
<br />
The most common execution models are:<br />
<ul style="text-align: left;">
<li>Offload Execution Mode</li>
<li>Coprocessor Native Execution Mode</li>
<li>Symmetric Mode</li>
</ul>
<br />
<br />
<table cellpadding="0" cellspacing="0" class="tr-caption-container" style="float: left; margin-right: 1em; text-align: left;"><tbody>
<tr><td style="text-align: center;"><a href="http://2.bp.blogspot.com/-A1mGAoWVxF4/VLn2cAInDJI/AAAAAAAACKo/bBu_P5FlGoQ/s1600/execution%2Bmodes.png" imageanchor="1" style="clear: left; margin-bottom: 1em; margin-left: auto; margin-right: auto;"><img border="0" height="304" src="http://2.bp.blogspot.com/-A1mGAoWVxF4/VLn2cAInDJI/AAAAAAAACKo/bBu_P5FlGoQ/s1600/execution%2Bmodes.png" width="640" /></a></td></tr>
<tr><td class="tr-caption" style="text-align: center;">Intel Xeon Phi Execution Modes</td><td class="tr-caption" style="text-align: center;"><br /></td><td class="tr-caption" style="text-align: center;"><br /></td><td class="tr-caption" style="text-align: center;"><br /></td><td class="tr-caption" style="text-align: center;"><br /></td><td class="tr-caption" style="text-align: center;"><br /></td><td class="tr-caption" style="text-align: center;"><br /></td></tr>
</tbody></table>
<br />
<div>
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<span style="color: red;">5. What is the Offload execution mode?</span><br />
<br />
<span style="color: red;"><span style="color: black;">The Offload execution model is also known as heterogeneous programming mode, here the host system offloads part or all of the computation from one or multiple processes or threads running on host. The application starts execution on the host. As the computation proceeds it can decide to send data to the coprocessor and let that work on it and the host and the coprocessor may or may not work in parallel. This is the common execution model in other coprocessor operating environment.</span></span><br />
<br />
<br />
<span style="color: red;"><span style="color: black;"></span></span><span style="color: red;"><span style="color: black;"><span style="color: red;">6. What is the Coprocessor native execution mode?</span></span></span><br />
<br />
<span style="color: red;"><span style="color: black;"><span style="color: red;"><span style="color: black;">Intel Xeon Phi hosts a Linux micro OS in it and can appear as another machine connected to the host like another node in a cluster. This execution environment allows the users to view the coprocessor as another compute node. In order to run natively, an application has to be cross compiled for Xeon Phi operating environment. Intel® Composer XE provides simple switch to generate cross compiled code.&nbsp;&nbsp;&nbsp;</span></span></span></span><br />
<br />
<br />
<span style="color: red;"><span style="color: black;">&nbsp;</span></span><span style="color: red;"><span style="color: black;"><span style="color: red;">7. What is the symmetric execution mode?</span></span></span><br />
<br />
<span style="color: red;"><span style="color: black;"><span style="color: red;"><span style="color: black;">In this case the application processes run on both the host and the Intel Xeon Phi<span style="color: red;"> </span>coprocessor. They usually communicate through some sort of message passing interface like MPI. This execution<span style="color: red;"> </span>environment treats Xeon Phi card as another node in a cluster in a heterogeneous cluster environment.&nbsp;&nbsp;</span></span></span></span><br />
<br />
<span style="color: red;"> </span><br />
<b><br /></b>
<b>References:</b><br />
<br />
https://software.intel.com/en-us/mic-developer<br />
<br /></div>
</div>
<div dir="ltr" style="text-align: left;" trbidi="on">
<div>
The following links and documents contain good examples and guidelines for a novice when programming for the Intel Xeon Phi.<br />

 <style type="text/css">p { margin-bottom: 0.25cm; line-height: 120%; }</style>

<br />

</div>
<a href="http://software.intel.com/sites/default/files/article/335818/intel-xeon-phi-coprocessor-quick-start-developers-guide.pdf">http://software.intel.com/sites/default/files/article/335818/intel-xeon-phi-coprocessor-quick-start-developers-guide.pdf</a><br /><br />
<br /><a href="http://software.intel.com/en-us/articles/building-a-native-application-for-intel-xeon-phi-coprocessors">http://software.intel.com/en-us/articles/building-a-native-application-for-intel-xeon-phi-coprocessors</a><br /><br />
<br /><a href="http://www.drdobbs.com/parallel/programming-intels-xeon-phi-a-jumpstart/240144160">http://www.drdobbs.com/parallel/programming-intels-xeon-phi-a-jumpstart/240144160</a><br /><br />
<br /><a href="http://www.prace-project.eu/IMG/pdf/Best-Practice-Guide-Intel-Xeon-Phi.pdf">http://www.prace-project.eu/IMG/pdf/Best-Practice-Guide-Intel-Xeon-Phi.pdf</a><br /><br />
<br /><a href="http://software.intel.com/sites/default/files/article/366893/offload-runtime-for-the-intelr-xeon-phitm-coprocessor.pdf">http://software.intel.com/sites/default/files/article/366893/offload-runtime-for-the-intelr-xeon-phitm-coprocessor.pdf</a><br /><br />
<br /><a href="http://research.colfaxinternational.com/file.axd?file=2013%2F5%2FColfax_Static_Libraries_Xeon_Phi.pdf">http://research.colfaxinternational.com/file.axd?file=2013%2F5%2FColfax_Static_Libraries_Xeon_Phi.pdf</a><br /><br />
<br /><a href="https://hpcforge.org/plugins/mediawiki/wiki/pracewp8/images/6/68/XeonPhi.pdf">https://hpcforge.org/plugins/mediawiki/wiki/pracewp8/images/6/68/XeonPhi.pdf</a><br /><br />
<br /><a href="http://software.intel.com/en-us/articles/getting-started-with-openmp">http://software.intel.com/en-us/articles/getting-started-with-openmp</a><br /><a href="https://www.blogger.com/goog_318173798">&nbsp;</a><br /><a href="http://d3f8ykwhia686p.cloudfront.net/1live/intel/An_Introduction_to_Vectorization_with_Intel_Compiler_021712.pdf">http://d3f8ykwhia686p.cloudfront.net/1live/intel/An_Introduction_to_Vectorization_with_Intel_Compiler_021712.pdf</a><br /><div>

<div style="text-align: left;">
</div>
</div>
</div>


