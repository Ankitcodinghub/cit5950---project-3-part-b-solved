# cit5950---project-3-part-b-solved
**TO GET THIS SOLUTION VISIT:** [CIT5950 – Project 3 Part b Solved](https://www.ankitcodinghub.com/product/cit5950-project-3-part-b-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114419&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CIT5950 - Project 3 Part b Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (1 vote)    </div>
    </div>
<h1><a name="_Toc21845"></a>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Project 3b: Multi-threaded Server</h1>
Overview

In this part, you will enhance your TCP server in Part A (tcpserver), such that the new server

(multi-tcpserver) can handle multiple concurrent client requests using <em>multi-threading</em>. In the server, when a client connection is accepted (via the accept API), the server should create a separate thread to handle the Handshake Protocol using the socket descriptor returned by the accept call. We have provided a sample C program for multi-threading (sample_thread.c) in the course module in which you learned threads.

Conceptually, Part B is just a refactoring effort from Part A. You would be putting all the client communication code into a thread function, which should be passed into pthread_create.

<h2><a name="_Toc21846"></a>1.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Requirements</h2>
<h3><a name="_Toc21847"></a>1.1.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Source files and arguments</h3>
All of the requirements from Part A remain the same, with the following changes:

<ul>
<li>You MUST implement the server in multi-tcpserver.c instead of tcpserver.c • The makefile MUST create the executable multi-tcpserver instead of tcpserver</li>
<li>You MUST link the pthread library (you will get a compile error if you forget!).</li>
</ul>
<h3><a name="_Toc21848"></a>1.1.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Handshake Protocol</h3>
All of the requirements from Part A apply to Part B.

<h3><a name="_Toc21849"></a>1.1.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; End of Line characters</h3>
All of the requirements from Part A apply to Part B.

<h3><a name="_Toc21850"></a>1.1.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Multi-threading</h3>
<ul>
<li>You MUST use multi-threading for this part. The autograder will do a static analysis to ensure you call the appropriate functions. See the The Autograder section below for details on this analysis.</li>
<li>Your multi-thread MUST handle interleaving correctly. This means that clients may send messages out of order, e.g. Client A may send HELLO X followed by Client B sending HELLO Y. See the Testing Interleaving section below for how to do this locally.</li>
<li>Threads should run as detached threads. Calling pthread_join can lead to non-concurrent operations and MUST NOT be used.</li>
</ul>
<h3><a name="_Toc21851"></a>1.1.5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Miscellaneous</h3>
<ul>
<li>You SHOULD reuse the client from Part A. You do not need to make any changes to the client for this part (unless there are still bugs).</li>
<li>You MAY assume that no more than 100 concurrent client connections will attempt to connect to the server.</li>
<li>All of the requirements from Part A apply to Part B.</li>
</ul>
<h2><a name="_Toc21852"></a>1.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Suggested Approach</h2>
This is a suggested approach. You are free to implement the solution in any manner you want.

<ol>
<li>Start by copying your Part A server code into the new source file.</li>
<li>If you haven’t already done so, refactor your code such that all of the handshake functionality is in a new helper function. What should be left is a small loop that accepts connections and then calls the helper function for the handshakes. Your server should still work as a sequential server at this point.</li>
<li>You’ll want to create an array of thread IDs, this will allow you to keep track of threads as they are created and destroyed. You only need to do this once.</li>
<li>Replace the call to the helper function with a call to pthread_create, with the helper function as an argument. Be sure to read the manual pages to ensure you setup the call correctly. Store the thread ID into the thread ID array.</li>
<li>Test your multi-threaded server by running a client. You should see all the handshakes print as expected.</li>
<li>Further test your multi-threaded server by running several clients back to back, sequentially. You should see each set of clients print the appropriate messages, in order.</li>
<li>Stress test your multi-threaded server by running several clients concurrently. The messages may print out of order due to interleaving. See the Testing Interleaving section below.</li>
</ol>
<h2><a name="_Toc21853"></a>1.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Submission</h2>
<ul>
<li>Your solution MUST compile when running make clean followed by make. Please do check this before submitting. Submissions that fail to compile will receive a 0.</li>
<li>You MUST submit all source and header files, and the makefile, in a tarball (.tar.gz) to the Gradescope assignment CIT 5950 Project 3b.</li>
<li>Your tarball SHOULD NOT contain compiled binaries or demo code files. • You have unlimited submissions until the due date specified by the syllabus.</li>
</ul>
<h2><a name="_Toc21854"></a>1.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Grading</h2>
Project 3b will be marked on five rubric items. The descriptions for these tests are in the The Autograder section.

There is no peer review for this assignment. You will not be marked on code style.

The score at the due date is final. Do note that they do not sync with Canvas immediately; the course staff must manually release them.

<ol>
<li>Static Analysis : 0 points</li>
<li>Proxy Test : 20 points</li>
<li>Load Test : 30 points</li>
<li>Interleaving Clients Test : 30 points</li>
<li>Server Error Checking Test : 20 points</li>
</ol>
Total : 100 points
