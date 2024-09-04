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
