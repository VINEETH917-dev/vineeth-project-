﻿# vineeth-project-
 # On the Effectiveness of Adaptive Lossless Image Compression Employing Huffman Encoding

## Project Overview
This project integrates an adaptive lossless image compression algorithm utilizing Huffman Encoding. The first aim is to provide a fast and accurate method of compressing grayscale images where image quality is preserved during both encoding and decoding phases.

## Objectives
Create a flexible lossless image compression and decompression approach by Huffman Encoding.
As used for grayscale images, improve the rate of achieving the ideal data compression factor without significant loss of data quality.
- Compare the compression ratio ad and the encoding/decoding durations, and the precision of the decompression.

## Key Concepts
- Huffman Encoding: An example of lossless coding techniques that assigns short code to frequently occurring symbols (pixel values) and long code to less frequently occurring symbols.
- Adaptive Huffman Encoding: An image encoding technique that is an enhanced version of the Huffman algorithm and the coding tree is changed as the image is being encoded.

## Methodology
1. Encoding Process:
   The image is converted into grayscale and array list and then this array list is converted into numpy array format.
   The number of times of occurrence of specific pixel values is counted, Huffman tree based on the priority queue is then developed.
   The picture elements are exchanged for Huffman codes of the same pixel.

2. Decoding Process:
   The compressed bitstream is then, decoded utilizing Huffman tree.
   Pixel values are then obtained from the binary bit stream and the original image is reconstructed without any loss.

## Performance Evaluation
- Compression Ratio: The average compression ratio of algorithm found to be of **1.16 : 1*. This is very much a function of the image content where by the simpler images are more easily compressed than others.
- Encoding Time: More specifically, the encoding time is somehow dependent with the intricacy and size of the image in question. The building of the Huffman tree is a computational process, or in other words it is costly.
- Decoding Time: Decoding can be done much faster as all you are giving is just the encoded text and the only thing you have to do is navigate through the constructed Huffman tree. 
## Graphical Results
Curves of the compression ratios were introduced indicating that the amount of detail in the images had a determinant relationship to the compression ratio achieved.
This analysis concluded that an improved compression ratio was attained for images with large homogeneous areas than for complex ones with high entropy.

## Decompression Accuracy
The algorithm effectively separates out the packaged images so that no information is lost as with more complicated or diverse images.
The quality of its decompressed images is then checked at a meta-pixel level to ensure that the compression is entirely lossless.

## Future Work
- They should consider studying more about parallel processing or even the use of GPU in an effort of reducing the encoding time.
Research other lossless algorithms that are out there among them being Arithmetic Coding or Lempel–Ziv–Welch (LZW).
Adding an interface makes it easier to use for non-technical personnel, especially as they only interact with Graphical User Interface (GUI).
Figure out how to adapt it into handling of color images and bigger sample sizes.
