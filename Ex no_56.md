# EX 56 C function to display stack elements using Linked List.(store integer data in stack) .
## DATE: 19/05/25
## AIM:
To write a C function to display stack elements using Linked List.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output 

## Program:
```
/*
C function to display stack elements using Linked List.(store integer data in stack) .

Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>
#include <stdlib.h>

typedef struct Node {
    int data;
    struct Node *next;
} Node;

void display(Node *top) {
    Node *temp = top;
    if (temp == NULL) {
        printf("Stack is empty\n");
        return;
    }
    while (temp != NULL) {
        printf("%d ", temp->data);
        temp = temp->next;
    }
    printf("\n");
}

## Output:

30 20 10

## Result:
Thus the program was executed and the output was verified successfully.
