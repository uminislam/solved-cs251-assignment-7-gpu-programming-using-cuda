Download Link: https://assignmentchef.com/product/solved-cs251-assignment-7-gpu-programming-using-cuda
<br>



<strong>Q1 [Understanding 2-D blocks] </strong>

Modify the ​<strong>pargpu.cu</strong>​ code (from the class examples) where number of threads are specified as a two dimensional variable. In CUDA, ​<strong>dim3</strong>​ data type can be used to specify two or three dimensional elements. Specifically, number of threads in each dimension of a 2-D block should be parameters to the program. Your program should be executed as follows,




$ ./q1 {number of elements} {rows} {cols}




Where rows * cols  &lt;= 1024 (max threads per block}

<strong> </strong>

<strong>Q2 [XOR based Checksum] </strong>

Given randomly generated N numbers {X​1, X<sub>​</sub>​2, …..X<sub>​ </sub>​N}<sub>​</sub> as input, find out the XOR sum as follows,

SUM = X​1 XOR X<sub>​ </sub>​2 XOR X<sub>​ </sub>​3 ….. XOR X<sub>​ </sub>​N




You can use maximum O(1) extra space to perform the operations on GPU. Further, the input copied to the device memory is not required to maintain the old values after completion of the program.




Your program should take two arguments, i.e., ​<em>number of elements</em>​ and a ​<em>random seed</em>​ as command line parameter. In your program (main function) should execute ​<strong>srand (seed)</strong>​ and generate random inputs before invoking the GPU kernel (refer class examples). Your program should print the final output in the console.