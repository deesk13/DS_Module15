# Ex12 Binary Search Tree
## DATE:25-05-25
## AIM:
To write a C function to insert the elements in the binary search tree

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to insert the elements in the binary search tree
Developed by: DEVA DHARSHINI
RegisterNumber:212223240026
/*structnode{
int key;
struct node*left, *right;
};*/
struct node* insert(struct node* node, int key)
{
if(node==NULL)
{
struct node*node=(struct node*)malloc(sizeof(struct node));
node->key=key;
node->left=NULL;
node->right=NULL;
return node;
}
else
{
struct node* cur;
if(key<=node->key)
{
cur=insert(node->left,key);
node->left=cur;
}
else
{
cur=insert(node->right,key);
node->right=cur;
}
returnnode;
}
}
 
*/
```

## Output:



## Result:
Thus, the C function to insert the elements in the binary search tree is implemented successfully.
