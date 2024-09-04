Three way Partitioning of an Array around a Given Range in Python
Here, on this page, we will discuss the program for the Three way Partitioning of an Array around a Given Range in Python programming language. We are given an array and a range say [low, high], we need to partition the array in such a way,

All the elements less than low value, should come first.
Elements between the low and high value come in middle.
All elements greater than high should come at the last.
Python program for Three way Partitioning of an Array around a Given Range
Algorithm
Initialize 3 empty arrays to store elements smaller than the given range, elements greater than the given range, elements between the given range
Iterate through the array using the variable i
If i is greater than l append it to lm
else-if i is greater than h append it to hm
Else append it to mm
Return the combination of all three arrays ( lm + mm + hm )
Three way Partitioning of an Array around a Given Range in Python
Python Code
Run
def partition(arr, l, h):
    lm = []
    mm = []
    hm = []
    for i in arr:
        if i < l:
            lm.append(i)
        elif i > h:
            hm.append(i)
        else:
            mm.append(i)
    return lm + mm + hm


array = [1, 17, 22, 16, 13, 5, 43, 18, 3, 10]
lowVal = 14
highVal = 20
print("After Partitioning :", partition(array, lowVal, highVal))
Output
After Partitioning : [1, 13, 5, 3, 10, 17, 16, 18, 22, 43]
