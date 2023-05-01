Download Link: https://assignmentchef.com/product/solved-embsys105-assignment-2-contextswitch
<br>
The goal of this assignment is to gain understanding of context switching by writing context switch code in assembly language.

<ol>

 <li>Download and unzip the ContextSwitch project contained in the zip file: ContextSwitch.zip</li>

 <li>Open the ContextSwitch.eww workspace in the EWARM IDE.</li>

 <li>Make sure the ContextSwitch project builds.</li>

 <li>Launch TeraTerm (38400 Baud rate)</li>

 <li>Build and upload the project and start it running.</li>

 <li>Break into the program to stop the output stream on the UART.</li>

 <li>Notice it is printing an endless stream of messages from task one like this:</li>

</ol>

University of Washington – Context Switch Application task one: 0 task one: 1 task one: 2 task one: 3

…

<ol start="8">

 <li>Implement the context switch code specified by the comments in switch.s.</li>

 <li>When completed correctly you should see output in the UART from both task one and task two as the context switches at every clock tick.</li>

</ol>

10.Clean your completed project and zip it into a file named

ContextSwitch_&lt;YourUwNetId&gt;.zip

<ol>

 <li>Clean means delete the “Debug” folder before zipping so you don’t bloat your submission.</li>

 <li>Example submission filename: uDebugger_johndoe.zip 11.Submit your zip file by the due date.</li>

</ol>

<strong>Optional Additional challenge!</strong>

Those looking for an additional challenge may want to implement testAndSet(). Implement it in assembly language using LDREX and STREX. Call it in the C code of each task to protect access to the UART so each task can print an entire line without interference. You may want to remove the print statement in the scheduler routine.