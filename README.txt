Student Name:	Aditya Gupta
UNCC ID:	800966229
Programming language: Python 3.5.2
Compiler:	MSC v.1900 32 bit (Intel)
Algorithm:	LZW
Files: 		encoder.py and decoder.py


This program requires user input as a python file name, 
an input text file name and bit length through command line.

Encoding:
The input data is encoded using the encoder.py file,
the dictionary of size 256 is built and initialized,
using the python dictionary data structure
in the dictionary, key are characters and values are the ascii values
the lzw compression algorithm is applied and we get the compressed data,
the program outputs the compressed data and stores it to an 
output file named inputFileName.lzw
The compressed data is of 2 bytes.

Decoding:
The compressed data is decompressed using the decoder.py file,
the dictionary of size 256 is built and initialized,
using the python dictionary data structure
in the dictionary, key are characters and values are the ascii values
the lzw decompression algorithm is applied and we get the decompressed data,
the program outputs the decompressed data and stores it to an 
output file named inputFileName_decoded.txt

How to run the file:
1. Open the command window.
2. Set the current directory to the location where the file is present.
3. To encode, type: 
	python encoder.py <inputFileName.txt> <number of Bits>

4. To decode, type:
	python decoder.py <inputFileName.lzw> <number of Bits>

The compressed file will be stored as inputFileName.lzw and the output 
file will be stored as inputFileName_decoded.txt

The program works well with both the examples provided on canvas, 
for other data the efficiency depends on the the repeating data values
and the size of data.