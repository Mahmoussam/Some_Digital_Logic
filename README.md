# Some_Digital_Logic
implementing some digital logic circuits and ideas for fun! &lt;and knowledge ofc>
## The content is only organized by the date, oldest first.
##### Table of Contents  
[4-bit JK counter](#4bitcounter)  
[5-bit Ring counter D ff](#ringcounter)
[assignment](#hw1)
[Hardware counter](#hardwarecounter)
[4*4 memory](#mem)
[4-bit Gray code counter](#gray)

<a name="4bitcounter"/>
## 4-Bit Synchronous Counter using JK flip flops
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/4-Bit%20sync%20counter.gif)
Reference: Essentials of Computer Organization and Architecture, Third Edition.
<a name="ringcounter"/>
## 5-Bit Ring counter using D flip flops
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Ring%20counter.gif)
Reference: Essentials of Computer Organization and Architecture, Third Edition.
<a name="hw1"/>
## a basic CUFE assignment using logic gates to implement a function.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%202.jpg)
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%201.jpg)
the arduino is just my 5V power source.
<a name="hardwarecounter"/>
## a basic 2 bit counter using JK ff
Using :
```
  -the fact that when j=H and k=H , Q(t+1)=Q(t)`
  -the clock of a bit is the Q of the previous bit, clk_i=Q_(i-1).
  -the main clock ,clk_0 , is achieved using 555 providing ~0.5 HZ
```
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%203.jpg)
<a name="mem"/>
## 4*4 memory !
an exercise given by my favorite book <can you guess?>
the circuit file is provided as well (logisim)
The idea is to use a decoder to enable the desired word at the memory grid , output its content on the output pins,
and using "write enable" we can write desired input into the activated 4-bit D flip flops word.
ofc the whole thing is synchronized with the clock. a video may be provided soon.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Screenshot%202023-10-31%20203640.png)
<a name="gray"/>
##Gray-counter?!
a 4-bit gray code counter based on
```G=B xor (B>>1)``
where xor is the bitwise `xor` operation and `>>` is the right shift bitwise operation
I got the idea from K-maps using gray codes for numbering.
please note that J-K used at this circuit is falling edge triggered.
circuit file is also provided "D.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Screenshot%202023-11-01%20123302.png)

