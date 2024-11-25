# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice." 

Given that I am able to setup a testing environment I would start off with the most basic operating system and options to run the code, reducing any possible confounding aspects to a theoretical zero. 
From there I should be able to underclock the system (which realistically is not necessary, but would help in analysis) such that I am able to input one value and then a two value list in order to directly compare their speeds. 
If the algorithm itself is in fact $O(n)$ then this should be able to give me an automatic confirmation, but for the sake of theory, comparing a list of four values to a list of two values should take twice as long and so on.
As noted in class, nlogn is the fastest an algorithm can run, as the possible combination of values contained within an array of length n will always be at minimum n!. Thus to even surpass that would require the algorithm to somehow make the number of combinations less than n!.
Which for an arbitrary set of inputs is impossible, at least repeatedly impossible.
