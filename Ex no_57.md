# EX 57 C function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)
## DATE:19/05/25
## AIM:
To write a C function to perfom push,pop and peek functions in Stack using Linked List.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output
## Program:
```
/*
function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)

Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>
#include <stdlib.h>

typedef struct Node {
    float data;
    struct Node *next;
} Node;

void push(Node **top, float value) {
    Node *newNode = (Node *)malloc(sizeof(Node));
    newNode->data = value;
    newNode->next = *top;
    *top = newNode;
}

void pop(Node **top) {
    if (*top == NULL) {
        printf("Stack underflow\n");
        return;
    }
    Node *temp = *top;
    *top = (*top)->next;
    free(temp);
}

void peek(Node *top) {
    if (top == NULL) {
        printf("Stack is empty\n");
        return;
    }
    printf("Top element: %.2f\n", top->data);
}


## Output:

Top element: 15.70



## Result:
Thus the program was executed and the output was verified successfully.
