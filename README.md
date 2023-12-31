# Some_Digital_Logic
implementing some digital logic circuits and ideas for fun! &lt;and knowledge ofc>
## Table of content so far:
[[4-Bit Synchronous Counter using JK flip flops]](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#4-bit-synchronous-counter-using-jk-flip-flops) 

[[5-Bit Ring counter using D flip flops]](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#5-bit-ring-counter-using-d-flip-flops)

[[a basic CUFE assignment using logic gates to implement a function.]](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#a-basic-cufe-assignment-using-logic-gates-to-implement-a-function)

[a basic 2 bit counter using JK ff](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#a-basic-2-bit-counter-using-jk-ff)

[4*4 memory !](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#44-memory-)

[Gray-counter?!](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/README.md#gray-counter)


## 4-Bit Synchronous Counter using JK flip flops
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/4-Bit%20sync%20counter.gif)
Reference: Essentials of Computer Organization and Architecture, Third Edition.

## 5-Bit Ring counter using D flip flops
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Ring%20counter.gif)
Reference: Essentials of Computer Organization and Architecture, Third Edition.

## a basic CUFE assignment using logic gates to implement a function.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%202.jpg)
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%201.jpg)
the arduino is just my 5V power source.

## a basic 2 bit counter using JK ff
Using :
```
  -the fact that when j=H and k=H , Q(t+1)=Q(t)`
  -the clock of a bit is the Q of the previous bit, clk_i=Q_(i-1).
  -the main clock ,clk_0 , is achieved using 555 providing ~0.5 HZ
```
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/digital%203.jpg)

## 4*4 memory !
an exercise given by my favorite book <can you guess?>
the circuit file is provided as well (logisim)
The idea is to use a decoder to enable the desired word at the memory grid , output its content on the output pins,
and using "write enable" we can write desired input into the activated 4-bit D flip flops word.
ofc the whole thing is synchronized with the clock. a video may be provided soon.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Screenshot%202023-10-31%20203640.png)

## Gray-counter?!
a 4-bit gray code counter based on
```G=B xor (B>>1)``
where xor is the bitwise `xor` operation and `>>` is the right shift bitwise operation
I got the idea from K-maps using gray codes for numbering.
please note that J-K used at this circuit is falling edge triggered.
circuit file is also provided "D.
![](https://github.com/Mahmoussam/Some_Digital_Logic/blob/master/Screenshot%202023-11-01%20123302.png)

