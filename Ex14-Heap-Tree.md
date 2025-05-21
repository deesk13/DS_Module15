# Ex14 Heap Tree
## DATE:21-05-25
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
```
1.Start and find the index of num in the array.
2.Swap num with the last element.
3.Decrease the array size by 1.
4.Heapify from the last non-leaf node (size/2 - 1) upwards.
5.End after restoring the heap property.
```
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: DEVA DHARSHINI
RegisterNumber:212223240026

void deleteRoot(int array[], int num)
{
int i;
for(i=0;i<size;i++)
{
if(num==array[i])
{
break;
}
}
swap(&array[i],&array[size-1]);
size-=1;
for(i=size/2-1;i>=0;i--)
{
heapify(array,size,i);
}
} 
*/
```

## Output:

![Screenshot 2025-05-21 140726](https://github.com/user-attachments/assets/2c2dc6de-9ed0-46af-8865-ee41a0c9e3a5)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
