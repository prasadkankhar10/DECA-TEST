4 1*8 8*1 
https://www.engineersgarage.com/vhdl-tutorial-14-design-1x8-demultiplexer-and-8x1-multiplexer-using-vhdl/

We shall write a VHDL program to build 1×8 demultiplexer and 8×1 multiplexer circuits
Verify the output waveform of the program (digital circuit) with the truth table of these multiplexer and demultiplexer circuits
1×8 Demultiplexer circuit

VHDL

Truth Table
(Please go through step by step procedure given in VHDL-tutorial 3 to create a project, edit and compile the program, create a waveform file, simulate the program, and generate output waveforms.)Now we shall write a VHDL program, compile it, simulate it, and get the output in a waveform. Finely, we shall verify that the output waveforms with the given truth table.

I have used the behavioral modeling style to write a VHDL program to build demultiplexer because it will be easier than the dataflow or structural modeling style.

VHDL Program



 (To know more and get more details about VHDL program(s), please go through the first two tutorials, VHDL tutorial 1 and VHDL tutorial 2 of these series.)

Next, compile the above program – create a waveform file with all inputs and outputs listed – apply different input combinations – save the waveform file, and finally, simulate the project. You will get the following result.

Simulation Waveform



As shown in the figure, one can observe that when select lines (S2, S1, S0) are “001”, the input I=0 is available in output O1=0, and when select lines are “101”, the input I=1 is available in output O5 = 1. You may verify other select line combinations with input and output.

Next, let us move on to build an 8×1 multiplexer circuit.



5 Flip Flop 

https://www.electronicsforu.com/technology-trends/learn-electronics/flip-flop-rs-jk-t-d

Table of Content
Flip-Flop v/s Latch
Flip-Flop Types
SR Flip-Flop
JK Flip-Flop
D Flip-Flop
T Flip-Flop
Applications
People Also Ask
Flip-Flop v/s Latch
The primary difference between a latch and a flip-flop is a gating or clocking mechanism.

- Advertisement -

In Simple words. Flip Flops are edge-triggered and a latch is level-triggered.

If you are confused between latch and flip-flop, then you should check this detailed article where we discussed the difference between Latch and flip-flop.

For example, let us talk about SR latch and SR flip-flops. In this circuit when you Set S as active, the output Q will be high and Q’ will be Low. This is irrespective of anything else. (This is an active-low circuit; so active here means low, but for an active high circuit, active would mean high)

SR latch Circuit Diagram
SR Latch
A flip-flop, on the other hand, is a synchronous Circuit and is also known as a gated or clocked SR latch.

SR Flip Flop Circuit
SR Flip Flop Circuit
In this circuit diagram, the output is changed (i.e. the stored data is changed) only when you give an active clock signal. Otherwise, even if the S or R is active, the data will not change. 

Let’s understand the flip-flop in detail with the truth table and circuits.

Flip Flop Types
There are 4 types of flip-flops in digital electronics:

SR Flip-Flop
JK Flip-Flop
D Flip-Flop
T Flip-Flop
Let’s understand each Flip-flop one by one.

1. SR Flip Flop
This is the most common flip-flop among all. This simple flip-flop circuit has a set input (S) and a reset input (R). In this system, when you Set “S” as active, the output “Q” would be high, and “Q‘” would be low. Once the outputs are established, the wiring of the circuit is maintained until “S” or “R” goes high, or power is turned off.

As shown above, it is the simplest and easiest to understand. The two outputs, as shown above, are the inverse of each other. The truth table of SR Flip-Flop is highlighted below.

S	R	Q	Q’
0	0	0	1
0	1	0	1
1	0	1	0
1	1	∞	∞
Recommended: SR Flip Flop Explained

2. JK Flip-Flop
Due to the undefined state in the SR flip-flops, another flip-flop is required in electronics. The JK flip-flop is an improvement on the SR flip-flop where S=R=1 is not a problem.

JK Flip Flop Circuit
JK Flip Flop Circuit
The input condition of J=K=1 gives an output inverting the output state. However, the outputs are the same when one tests the circuit practically.

In simple words, If J and K data input are different (i.e. high and low), then the output Q takes the value of J at the next clock edge. If J and K are both low, then no change occurs. If J and K are both high at the clock edge, then the output will toggle from one state to the other. JK Flip-Flops can function as Set or Reset Flip-flops.

JK FF Truth Table:
J	K	Q	Q’
0	0	0	0
0	1	0	0
1	0	0	1
1	1	0	1
0	0	1	1
0	1	1	0
1	0	1	1
1	1	1	0
Also Read: Everything you need to know about JK Flip Flop

3. D Flip-Flop
D flip-flop is a better alternative that is very popular with digital electronics. They are commonly used for counters, shift registers, and input synchronization.

D flip-flop Circuit Diagram
D Flip-Flop
In the D flip-flops, the output can only be changed at the clock edge, and if the input changes at other times, the output will be unaffected.

Truth Table:
Clock	D	Q	Q’
↓ » 0	0	0	1
↑ » 1	0	0	1
↓ » 0	1	0	1
↑ » 1	1	1	0
 The change of state of the output is dependent on the rising edge of the clock. The output (Q) is the same as the input and can only change at the rising edge of the clock.

Recommended: D Flip Flop Working and Applications

4. T Flip-Flop
A T flip-flop is like a JK flip-flop. These are single-input versions of JK flip-flops. This modified form of the JK is obtained by connecting inputs J and K together. It has only one input along with the clock input.

T flip flop circuit
T flip flop
These flip-flops are called T flip-flops because of their ability to complement their state i.e. Toggle, hence they are named Toggle flip-flops.

Truth Table:
T	Q	Q (t+1)
0	0	0
1	0	1
0	1	1
1	1	0
Also Read: T Flip Flop Working

Applications
These are the various types of flip-flops being used in digital electronic circuits and the applications of Flip-flops are as specified below.

Counters
Frequency Dividers
Shift Registers
Storage Registers
You can also check this PowerPoint presentation to learn more about Flip-flops in Digital Electronics.



8×1 multiplexer circuit



Truth Table


https://de-iitr.vlabs.ac.in/exp/multiplexer-demultiplexer/
