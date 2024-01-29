# GNU Radio Data Types
GNU Radio supports a number of data types that can be processed in the flograph. Each block indicates the data type a given port handels via the use of a handy colour scheme.<br>

A complete list of supported types and assigned colour scheme can be seen in the image below.
<br>

<img src="../img\GUI Screenshots\DataType_List.png" width="300px">

<br>

> Note: If you need a quick reminder of the supported types, goto:<br>
Help -> Types<br>
This option will show a handy list of supported and colour coded data types (as seen below).<br><br>
<img src="../img/GUI Screenshots/DataType_help_dropdown.png">

GNU Radio uses common data types that are identical to most programming languages.<br> 
These include:
* Float 64
* Float 32
* Integer 64 (long)
* Integer 32
* Integer 16 (short)
* Integer 8 (char)

There are some extra types are are more unique to GNU Radio, so require a little more explination here.

## Complex Types
Complex Types are a method of representing complex numbers which are commonly used in GNU Radio and genral signal processing.
<br><br>
Imaginary numbers are useful in signal processing as both magnitude and phase infomation can be found for any given sample.<br>
<br>
In the feild of Digital Signal Processing (DSP), data symbols are often encoded by changing (modulating) either the Phase, Magnitude, or Frequency of a transmitted signal (or a mixture diffrent modulation types).
>eg.<br> 
>Traditinal Radio Stations encode audio signals using either:<br>
>FM (Frequency Modulation) <br>or<br>
>AM (Amplitude Modulation)

Complex numbers consist of two components:
* Real Component
* Imaginary Component

They can be written mathmatically in "Rectangular Form" as follows:<br>
> Z = x + yi<br>

Where 'x' is the real component, y is the imaginary component (hence followed by i) and Z is the complex number.

> Note: the term 'i' is the square root of minus one. This is useful to know when multiplying imaginary numbers together.<br>
eg. <br>
Z = (1 + 2i) * (2 + 3i) <br>
Z = +2 +3i +4i -6 <br>
Z = -4 + 7i

### Finding the Magnitude of a Complex Sample

The magnitude of the complex number Z is usually written as |Z|.<br>
It can be found with the following formula.

>|Z| = |x + yi| <br>
>or<br> 
>|Z| = sqrt(x^2 + y^2)

eg. <br>

let: <br>
Z = 3 + 4i<br>
* |Z| = |3^2 + (4i)^2|<br>
* |Z| = |9 - 16|<br>
* |Z| = |-5|
* |Z| = 5

### Finding the Phase of a Complex Number
>Phase = arcTan(y/x)

let:<br>
Z = 3 + 4i

* Phase = arcTan(4/3)
* Phase = 53 degrees
* Phase = 0.295 Pi Radians

### Polar form of a Complex Number
Above we use 'Rectangular notation' to represent our complex number Z.<br>
Rectangular notation is the format that a complex sample is stored in.<br>
The draw back of this notation is that it requires calculation to find the phase and magnitude of a sample.<br>
<br>
Polar notation allows a mathmatition to imediatly identify both phase and magnitude infomation however, sacrificing the ease of viewing the real and imaginary components sepratly.<br>

In the above examples, we found the phase and magnitude of the complex number<br>
> Z = 3 + 4i<br>

To write this number in polar notation, do the following:
> Z = |Z| * e^(Phase)<br>
> Z = 5e^(0.295 Pi)

