Download Link: https://assignmentchef.com/product/solved-eecs2040-homework-1
<br>
<strong>Part 1</strong>

<ol>

 <li>(20%) Using the ADT1.1 <em>NaturalNumber</em> in the textbook pp.10, add the following operations to the <em>NaturalNumber</em> ADT: Predecessor, <em>IsGreater</em>, <em>Multiply</em>, <em>Divide</em>.</li>

 <li>(20%) Determine the frequency counts for all statements (by step table) in the following two program segments:</li>

</ol>

code (a):                           code (b)

<ul>

 <li>for(i=1;i&lt;=n;i++)                                     1  i=1;</li>

 <li>for(j=1;j&lt;=I;j++)                                     2  while(i&lt;=n)</li>

 <li>for(k=1;k&lt;=j;k++)                         3  {</li>

 <li>x++;                                                        4    x++;</li>

 <li>i++;</li>

 <li>}</li>

</ul>

<ol start="3">

 <li>(20%) For the function Multiply() shown below,

  <ul>

   <li>Introduce statements to increment count at all appropriate points and compute the count</li>

   <li>Simplify the resulting program by eliminating statement and compute the count</li>

   <li>Obtain the step count for the function using the frequency method.</li>

  </ul></li>

</ol>




void Multiply(int **a,int **b, int **c, int m, int n, int p)

{   for(int i=0;i&lt;m;i++)     for(int j=0; j&lt;p; j++)

{       c[i][j] = 0;       for(int k=0;k&lt;n;k++)        c[i][j] += a[i][k] * b[k][j];

}

}




<ol start="4">

 <li>(20%) A complex-valued matrix X is represented by a pair of matrices (A, B) where A and B contains real values. Write a program that computes the product of two complex-valued matrices (A, B) and (C, D), where (A, B) * (C, D) = (A+iB)*(C+iD) = (AC-BD)+i(AD + BC). Determine the number of additions and multiplications if the matrices are all nxn.</li>

 <li>(20%) The Tower of Hanoi is a classical problem which can be solved by recurrence. There are three pegs and N disks of different sizes. Originally, all the disks are on the left peg, stacked in decreasing size from bottom to top. Our goal is to transfer all the disks to the right peg, and the rules are that we can only move one disk at a time, and no disk can be moved onto a smaller one. We can easily solve this problem with the following recursive method: If N = 1, move this disk directly to the right peg and we are done. Otherwise (N &gt;1), first transfer the top N − 1 disks to the middle peg applying the method recursively, then move the largest disk to the right peg, and finally transfer the N −1 disks on the middle peg to the right peg applying the method recursively. Let T(N) be the total number of moves needed to transfer N disks.

  <ul>

   <li>Prove that T(N) = 2T(N −1) + 1 with T(1) = 1.</li>

   <li>Unfold this recurrence relation to obtain a closed-form expression for T(N). (T(N) is expressed in terms of function of N.)</li>

  </ul></li>

</ol>










<strong>Part 2 Coding </strong>You should submit:

<ul>

 <li>All your source codes (C++ file).</li>

 <li>Show the execution trace of your program.</li>

</ul>




<ol>

 <li>(30%) Write a C++ program to implement the <strong>3 Polynomial</strong> (pp.88) using</li>

</ol>

Representation 3 (dynamic array of (coef, exp) tuples). Implement the

Mult(Polynomial p) and Eval(float x). Estimate the computing time for Mult and Eval function. Add two more functions to input and output polynomials via <strong>overloading</strong> the <strong>&gt;&gt;</strong> and <strong>&lt;&lt; operators</strong>.

You should try out at least two runs of your program (execution trace) to <strong>demonstrate</strong> the Add, Mult, Eval and input, output functions.

<ol start="2">

 <li>(35%) Write a C++ program to implement the <strong>4 SparseMatrix</strong> in textbook (pp.97) (with Transpose implemented by FastTranspose). You should build you program based on the example codes in the book and implement the Add function and functions to input, output a sparse matrix by <strong>overloading</strong> the <strong>&gt;&gt;</strong> and <strong>&lt;&lt;</strong> <strong>operators</strong>.</li>

</ol>

You should try out at least two runs of your program to demonstrate the Add, Mult, Eval and input, output functions.

<ol start="3">

 <li>(35%) Write a C++ program to implement the <strong>5 String</strong> (pp.114) (with Find function implemented by FastFind). In addition, write two more functions:</li>

</ol>

String::Delete(int start, int length); //remove length characters beginning at start

String::CharDelete(char c); //returns the string with all occurrence of c removed. You should try out at least two runs of your program to demonstrate all those functions.