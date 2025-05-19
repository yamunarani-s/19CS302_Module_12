# EX 58 C Function to display queue elements using Linked List.(use integer data in the queue)
## DATE:19/05/25
## AIM:
To write a C Function to display queue elements using Linked List.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output
## Program:
```
/*
C Function to display queue elements using Linked List.(use integer data in the queue)

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

void display(Node *front) {
    if (front == NULL) {
        printf("Queue is empty\n");
        return;
    }
    Node *temp = front;
    while (temp != NULL) {
        printf("%d ", temp->data);
        temp = temp->next;
    }
    printf("\n");
}


## Output:

10 20 30

## Result:
Thus the program was executed and the output was verified successfully.
