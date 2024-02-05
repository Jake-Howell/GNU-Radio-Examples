# Converting an ASCII Text file to Unipolar Line Code
Converting an ASCII text file to Unipolar line code is a fundimental and useful task to understand when learning the basics of Digital Signal Processing (DSP) and GNU Radio.<br>
Once this task is fully understood, you will have your first continous data stream that can be used to modulate other signals with.<br>
<br>
In this section, we will cover the following:<br>

1. Using the File Source Block to read and output ASCII charachters 
2. Using the Packet to Unpacked Block to convert each byte of an ASCII Charachter to 8 individual bits.
3. Throtteling the Data Stream to limit processing to a specified sample rate (or baudrate) 
4. Using the Char to Float Type Coverter Block to transform the descreete value of a single bit, to a continuous value that is more useful for DSP techniques and Data Transmission.
5. Viewing the output using the QT GUI Time Sink Instrumentation block