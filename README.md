# softeng370-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [SOFTENG370 Assignment 3 Solved](https://www.ankitcodinghub.com/product/softeng370-assignment-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100656&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SOFTENG370 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="section">
<div class="layoutArea">
<div class="column">
Part 1

</div>
</div>
<div class="layoutArea">
<div class="column">
This part of the assignment is concerned with compiled executable files and how they are loaded into memory. There are many details involved in how this happens we are only going to look at some of them.

Compile the say_hello.c program. cc say_hello.c -o say_hello

Run it to make sure everything is ok.

./say_hello

For all of these instructions or questions show the relevant output you get when you run the commands. If there is a lot of output you should include the sections you need to answer the questions.

Programs compiled on modern Linux systems place executable and shared code into ELF files (Executable and Linkable Format). ELF files have a strict structure.

The first part of an ELF file is the header.

<pre>readelf -h say_hello
</pre>
<ol>
<li>1.a) &nbsp;What is the architecture the file is compiled to run on? [0.5]</li>
<li>1.b) &nbsp;What is the type? Why is the type not EXEC (executable – see man ELF)? [1]</li>
</ol>
The next parts are the segments.

<pre>readelf -l say_hello
</pre>
1.c) Using one sentence for each type, describe the different segment types you see. You do not need to describe the GNU extensions (starting with GNU). [2]

<ol start="4">
<li>1.d) &nbsp;From the output above or otherwise what is the interpreter in the ELF header? [0.5]</li>
<li>1.e) &nbsp;Given that the program is compiled why does it have an interpreter? [1]</li>
<li>1.f) &nbsp;In which of the program segments do you think the main function is stored? Give a reason. [1]</li>
</ol>
Sections are also important parts of an ELF file.

<pre>readelf -SW say_hello
</pre>
We will return to the sections in a later question. For the moment examine the output. You don’t need to include this in your submission.

1.g) Describe the main differences between how program segment headers and section headers in ELF files are used. Include any web links you used to find your answer. [2]

Now to look at the code stored in our ELF file.

For this section you are not expected to completely understand the assembly language code. Here

are just a few things to help. The LEA instruction loads an address into a register or memory page 1

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
SOFTENG 370 Assignment 3

</div>
</div>
<div class="layoutArea">
<div class="column">
location. The RDI register and other registers are used to pass integer parameters to functions when they are called.

e.g. lea 0xe6(%rip),%rdi

This works out the address by adding E6 to the current value of the instruction pointer (RIP – like the PC in other instruction sets). The RIP will always hold the address of the next instruction following this one. So if the next address is 654, the address stored by LEA in RDI will be 654 + E6 = 73A.

CALLQ is a function call. Because we want position independent code the destination address of all calls are relative to RIP.

The objdump command allows us to inspect the code in the ELF file.

<pre>objdump -d say_hello
</pre>
This disassembles the code inside the ELF file.

<ol>
<li>2.a) &nbsp;In the header information in question 1 one of the values is the entry point address for the file. Locate the disassembled instructions from the relevant section in the objdump output. Include them in your answer. [0.5]</li>
<li>2.b) &nbsp;In a general way (you don’t have to give details) explain how the main function is reached from this code. [2]</li>
<li>2.c) &nbsp;Show the assembly language which corresponds to the main function. [0.5]</li>
<li>2.d) &nbsp;When the main function returns, where does it return to? (In general, not the address.) [1]</li>
</ol>
Now look at the memory associated with the program as it runs. Start the program but leave it waiting for your input (and in another terminal get the process id via the ps a command). Process information is stored in the /proc directory.

If the process id is 18020 all the process information can be found in the /proc/18020 directory. 3.a) Find the regions of memory mapped to this process. Show the output. [0.5]

<pre>cat /proc/18020/maps
</pre>
3.b) See the files behind them. Show the output. [0.5]

<pre>ls -l /proc/18020/map_files/
</pre>
3.c) Comparing this information with information from the ELF file, where in memory was the main function when the program was running? Explain how you worked that out. [2]

Possible references:

https://en.wikipedia.org/wiki/Executable_and_Linkable_Format

https://www.cs.stevens.edu/%7Ejschauma/631/elf.html

https://lwn.net/Articles/631631/

Further information can be gathered from the man pages on readelf, and objdump. Also read the /proc/[pid]/maps section in man proc.

</div>
</div>
<div class="layoutArea">
<div class="column">
page 2

</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
SOFTENG 370 Assignment 3

</div>
</div>
<div class="layoutArea">
<div class="column">
Part 2

4. [4]

We can keep track of free memory in a similar way to free blocks on disk. We could use a bitmap where 1 bit represents a free frame of memory or we could maintain a linked list of free frames. The linked list is maintained as a list of nodes where each node has a frame number, and a pointer to the next node. Assume these pointers and numbers are 64 bits each.

Calculate the space requirements using each of those methods for the following system, give the answers in bytes:

32 GB (235 bytes) of RAM in 8 KB (213 bytes) frames. Assume that memory is currently being used in alternating chunks of size 1 MB (220 bytes). i.e. The first MB of RAM is used, the second is free, the third is used, etc.

How much of that space (for both approaches) would normally be in kernel memory? Why? How would an extents version compare to the two approaches in the question above?

5. [2]

The number of instructions executed between page faults is directly proportional to the number of page frames allocated to a program. Double the amount of memory allocated to a process and you double the length of time between page faults. Suppose that a normal instruction takes 1 nanosecond, but if a page fault occurs, it takes 1,000,000 nanoseconds (i.e. 1msec) to handle the fault. If a program which is allocated n page frames takes 100 seconds to run, during which time it gets 50,000 page faults, how many page frames should be allocated to the program in order to have it finish in 60 seconds? Explain your working.

6. [4]

Given a machine with 5 frames show the contents of each frame using the following replacement algorithms on the reference string. Also say how many page faults would occur for each algorithm. Pages are brought in on demand and the initial load of a page counts as a page fault.

<ol>
<li>a) &nbsp;FIFO – First In First Out</li>
<li>b) &nbsp;LRU – Least Recently Used</li>
<li>c) &nbsp;LFU – Least Frequently Used (if there are multiple pages with the same lowest frequency choose in a FIFO manner)</li>
<li>d) &nbsp;Optimal (if there are multiple pages which are not used again choose in a FIFO manner)</li>
</ol>
</div>
</div>
<table>
<tbody>
<tr>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td></td>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
0

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
Lay out your answer for each algorithm like this. A zero means the frame is free, an empty cell means the content of the frame is the same as in the previous step.

</div>
</div>
<div class="layoutArea">
<div class="column">
page 3

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
SOFTENG 370 Assignment 3

</div>
</div>
<div class="layoutArea">
<div class="column">
Submitting the assignment

Put all of the output requested and the answers to questions in a single file for upload via Canvas. The file must be readable to TurnItIn e.g. not an image (otherwise you may get zero for the assignment).

Make sure your name and upi is included in the file you submit.

Any work you submit must be your work and your work alone – see the School and University policies on academic integrity.

</div>
</div>
<div class="layoutArea">
<div class="column">
page 4

</div>
</div>
</div>
</div>
