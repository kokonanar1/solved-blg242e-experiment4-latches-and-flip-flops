Download Link: https://assignmentchef.com/product/solved-blg242e-experiment4-latches-and-flip-flops
<br>



In this experiment, you will implement and examine data storage elements: latches and flip-flops using Verilog. In this experiment, you are allowed to use ‘&amp;’ (Bitwise AND), ‘|’ (Bitwise OR), ‘∼’ (Bitwise NOT), ‘{}’ (Concatenate). Moreover, you can also use always block but only in the last part. That is, you are not allowed to implement latches and flip flops with this keyword. <em>You must simulate all parts separately with Vivado. </em>For this experiment, it may be useful to revise your previous knowledge from BLG231E-Digital Circuits course.

<h1>2 Preliminary</h1>

Answer the following questions in your report using your own words. Please be careful about not plagiarizing and properly cite the sources you benefit from.

<ol>

 <li>Explain what a flip flop is and why they are useful. Use your own words.</li>

 <li>Explain what are the differences between latches and flip flops with your own words.</li>

 <li>Briefly explain how an SR-latch works and what the functionalities of the input variables are.</li>

 <li>Construct the truth table of an SR latch which does not have an Enable input.</li>

 <li>Construct the truth table of an SR latch which has an Enable input.</li>

 <li>Construct the truth table of a D flip flop.</li>

</ol>

1

<em>Experiment 4: Latches and Flip Flops</em>

3 Experiment

<h1>Part 1 – SR Latch (only NAND Gates)</h1>

Please implement an SR latch module with S and R inputs and with <em>Q </em>and <em>Q neg </em>outputs <em>without an Enable input</em>. You are allowed to use only 2-input NAND gates that you should implement as a separate module. Using the truth table you have constructed in the Preliminary section, write the characteristic equation of the latch as <em>Q</em>(<em>t </em>+ 1) = <em>f</em>(<em>S</em>;<em>R</em>;<em>Q</em>(<em>t</em>)). In your report, explain how you found the equation and how the latch behaves for disallowed inputs.

<h1>Part 2 – SR Latch with Enable input (only NAND Gates)</h1>

Please implement an SR latch module with S, R and Enable inputs and with <em>Q </em>and <em>Q neg </em>outputs. You are allowed to use only 2-input NAND gates that you should implement as a separate module. Using the truth table you have constructed in the Preliminary section, write the characteristic function of the latch as <em>Q</em>(<em>t </em>+ 1) = <em>f</em>(<em>S</em>;<em>R</em>;<em>E</em>;<em>Q</em>(<em>t</em>)). In your report, explain how you found the equation and how the latch behaves for disallowed inputs. Discuss whether it is different from an SR Latch without an Enable input in your report.

<h1>Part 3 – D Flip-Flop from D-Latches</h1>

Please implement a positive edge triggered D flip-flop module with D input and for <em>Q </em>and <em>Q neg </em>outputs using D latches. You should implement the D latches yourselves using only 2-input NAND gates as a separate module. Show that the clock is only effective at rising edge.

<h1>Part 4</h1>

Please implement a positive edge triggered pulse generator using a circular shift register. The circuit should take 16-bit input for the loaded value, 1-bit input for the clock signal, 1-bit input for the load flag and give 1-bit output. Basically, when Load=0 (that is, shift=1), with the clock signal, circular shift operation is done; when Load=1, with the clock signal, a 16-bit input value is loaded.

Design your circuit in a way that the output of this circuit is the most significant bit (MSB) of the loaded value (so, firstly determine what the direction of the shift should be to maintain MSB as the output).

Your design should support variable pulse frequencies and duration listed below. Build the circuit and generate given signals. For each signal, observe both input and output.

2

Explain your findings on the report.

<ul>

 <li>with the 1/2 frequency of clock signal</li>

 <li>with the 1/4 frequency of clock signal</li>

 <li>with the 1/8 frequency of clock signal</li>

 <li>with 1/7 pulse-gap duration rate</li>

 <li>with 1/15 pulse-gap duration rate</li>

 <li>with 3/13 pulse-gap duration rate</li>

 <li>with 11/5 pulse-gap duration rate</li>

</ul>

<strong>Hint 1: </strong>You can analyze the internal structure of 74XX165 IC for pulse-generator.

<strong>Hint 2: </strong>You can check what Pulse Width Modulation (PWM) is.

<strong>Hint 3: </strong>In order to provide different frequency ratios with your pulse generator, you should change the 16-bit input values in the simulation step. You should not change the design of the pulse generator for different frequency ratios.