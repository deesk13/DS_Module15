# Ex15 Largest Element in BST
## DATE:20-05-25
## AIM:
To Write a c program to find the largest value in a Binary Search Tree.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: DEVA DHASRHINI
RegisterNumber:212223240026
#include <stdio.h>
#include <stdlib.h>
struct node
{
 int info;
 struct node *left, *right;
};
struct node *createnode(int key)
{
 struct node *newnode = (struct node*)malloc(sizeof(struct node));
 newnode->info = key;
 newnode->left = NULL;
 newnode->right = NULL;
 return(newnode);
}
void inorder(struct node *root)
{
 if(root != NULL)
 {
 inorder(root->left);
 printf(" %d ",root->info);
 inorder(root->right);
 }
}
void largest(struct node *root)
{
 while (root != NULL && root->right != NULL)
 {
 root = root->right;
 }
 printf("\nLargest value is %d", root->info);
}
EX.NO : 3(E)
LARGEST ELEMENT IN BST
DATE :
/*
* Main Function
*/
int main()
{
 /* Creating first Tree. */
 struct node *newnode = createnode(25);
 newnode->left = createnode(17);
 newnode->right = createnode(35);
 newnode->left->left = createnode(13);
 newnode->left->right = createnode(19);
 newnode->right->left = createnode(27);
 newnode->right->right = createnode(55);

 printf("Inorder traversal of tree 1 :");
 inorder(newnode);
 largest(newnode);

return 0;
}


*/
```

## Output:
![Screenshot 2025-05-21 140853](https://github.com/user-attachments/assets/cc3127f8-5289-4013-9e88-f2c840bae749)



## Result:
Thus, the C program to find the largest value in a Binary Search Tree is implemented successfully.
