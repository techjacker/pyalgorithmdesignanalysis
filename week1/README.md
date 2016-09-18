# Week 1

## Notes

#### Benchmarking
	- [go](http://dave.cheney.net/2013/06/30/how-to-write-benchmarks-in-go)
	- [go](https://coderwall.com/p/cp5fya/measuring-execution-time-in-go)
	- [python](http://stackoverflow.com/questions/2662140/how-to-measure-running-time-of-algorithms-in-python)

#### Merge Sort
	- Good	introduction to	divide & conquer
	- Improves over	Selection, Insertion, Bubble sorts
	- princeton [notes on merge sort](https://www.coursera.org/learn/introduction-to-algorithms/home/week/3)



-----------------------------------------------------------

## Optional Theory Problems

1. You are given as input an unsorted array of n distinct numbers, where n is a power of 2. Give an algorithm that identifies the second-largest number in the array, and that uses at most $$n +\log_2 n - 2$$ comparisons.

2. You are a given a unimodal array of n distinct elements, meaning that its entries are in increasing order up until its maximum element, after which its elements are in decreasing order. Give an algorithm to compute the maximum element that runs in O(log n) time.

3. You are given a sorted (from smallest to largest) array A of n distinct integers which can be positive, negative, or zero. You want to decide whether or not there is an index i such that A[i] = i. Design the fastest algorithm that you can for solving this problem.


-----------------------------------------------------------
## Programming Assignment

Download the following text file:IntegerArray.txt

This file contains all of the 100,000 integers between 1 and 100,000 (inclusive) in some order, with no integer repeated.

Your task is to compute the number of inversions in the file given, where the $$i^{th}$$ row of the file indicates the $$i^{th}$$ entry of an array.

Because of the large size of this array, you should implement the fast divide-and-conquer algorithm covered in the video lectures.

The numeric answer for the given input file should be typed in the space below.

So if your answer is 1198233847, then just type 1198233847 in the space provided without any space / commas / any other punctuation marks. You can make up to 5 attempts, and we'll use the best one for grading.

(We do not require you to submit your code, so feel free to use any programming language you want --- just type the final numeric answer in the following space.)

[TIP: before submitting, first test the correctness of your program on some small test files or your own devising. Then post your best test cases to the discussion forums to help your fellow students!]

Answer = ?


-----------------------------------------------------------
## Problem Set

#### 1.

3-way-Merge Sort : Suppose that instead of dividing in half at each step of Merge Sort, you divide into thirds, sort each third, and finally combine all of them using a three-way merge subroutine. What is the overall asymptotic running time of this algorithm? (Hint: Note that the merge step can still be implemented in $$O(n)$$ time.)

$$n ( \log(n))^2$$

$$n^2\log(n)$$

$$n$$

$$n \log(n)$$


#### 2.

You are given functions $$f$$ and $$g$$ such that $$f(n)=O(g(n))$$. Is $$f(n)*log_2(f(n)^c) = O(g(n)*log_2(g(n)))$$ ? (Here $$c$$ is some positive constant.) You should assume that $$f$$ and $$g$$ are nondecreasing and always bigger than 1.

Sometimes yes, sometimes no, depending on the constant $$c$$

Sometimes yes, sometimes no, depending on the functions $$f$$ and $$g$$

False

True


#### 3.

Assume again two (positive) nondecreasing functions $$f$$ and $$g$$ such that $$f(n)=O(g(n))$$. Is $$2^{f(n)}=O(2^{g(n)})$$ ? (Multiple answers may be correct, you should check all of those that apply.)

Never

Sometimes yes, sometimes no (depending on $$f$$ and $$g$$)

Yes if $$f(n) \le g(n)$$ for all sufficiently large $$n$$

Always


#### 4.

k-way-Merge Sort. Suppose you are given $$k$$ sorted arrays, each with $$n$$ elements, and you want to combine them into a single array of $$kn$$ elements. Consider the following approach. Using the merge subroutine taught in lecture, you merge the first 2 arrays, then merge the $$3^{rd}$$ given array with this merged version of the first two arrays, then merge the $$4^{th}$$ given array with the merged version of the first three arrays, and so on until you merge in the final ($$k^{th}$$) input array. What is the running time taken by this successive merging algorithm, as a function of $$k$$ and $$n$$? (Optional: can you think of a faster way to do the k-way merge procedure ?)

$$\theta(nk)$$

$$\theta(nk^2)$$

$$\theta(n \log(k))$$

$$\theta(n^2k)$$


#### 5.

Arrange the following functions in increasing order of growth rate (with $$g(n)$$ following $$f(n)$$ in your list if and only if $$f(n)=O(g(n))$$).

a)$$2^{2^n}$$

b)$$2^{n^2}$$

c)$$n^2\log(n)$$

d)$$n$$

e)$$n^{2^n}$$

Write your 5-letter answer, i.e., the sequence in lower case letters in the space provided. For example, if you feel that the answer is a->b->c->d->e (from smallest to largest), then type abcde in the space provided without any spaces before / after / in between the string.

You can assume that all logarithms are base 2 (though it actually doesn't matter).

WARNING: this question has multiple versions, you might see different ones on different attempts!
