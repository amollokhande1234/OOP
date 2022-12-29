
def selectionSort(nums):
    for i in range(5):
        minpos = i
        for j in range(i,6):
            if nums[j] < nums[minpos]:
                minpos = j
        temp = nums[i]
        nums[i] = nums[minpos]
        nums[minpos] = temp
        

def bubbleSort(nums):
    for i in range(len(nums)-1,0,-1):
        for j in range(i):
            if nums[j]>nums[j+1]:
                temp = nums[j]
                nums[j] = nums[j+1]
                nums[j+1] = temp
def topFiveMarks(nums):
    print("Top ",len(nums),"Marks are :) ")
    print(*nums[::-1],sep="\n")
    return ("Printed Successfully !")
           

nums = [85,23,98,67,52,70]
selectionSort(nums)
bubbleSort(nums)
topFiveMarks(nums)
print("Selectioin Sort :) ",nums)
print("Bubble Sort :) ", nums)
print(topFiveMarks(nums))