# EX 60 C function to find the peek element of the queue using linked list.
## DATE: 19/05/25
## AIM:
To write a C function to find the peek element of the queue using linked list.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output
## Program:
```
/*
C function to find the peek element of the queue using linked list.

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

int peek(Node *front) {
    if (front == NULL) {
        printf("Queue is empty\n");
        return -1; // or some error code
    }
    return front->data;
}

## Output:

Queue is empty


## Result:
Thus the program was executed and the output was verified successfully.
