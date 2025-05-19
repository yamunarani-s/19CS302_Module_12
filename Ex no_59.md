# EX 59 C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).
## DATE: 19/05/25
## AIM:
To write a C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output
## Program:
```
/*
functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).

Developed by: YAMUNA RANI S
RegisterNumber:  212223060309
*/
```
#include <stdio.h>
#include <stdlib.h>

typedef struct Node {
    char data;
    struct Node *next;
} Node;

void enqueue(Node **front, Node **rear, char value) {
    Node *newNode = (Node *)malloc(sizeof(Node));
    newNode->data = value;
    newNode->next = NULL;

    if (*rear == NULL) {
        *front = *rear = newNode;
        return;
    }

    (*rear)->next = newNode;
    *rear = newNode;
}

void dequeue(Node **front, Node **rear) {
    if (*front == NULL) {
        printf("Queue is empty\n");
        return;
    }
    Node *temp = *front;
    *front = (*front)->next;

    if (*front == NULL)
        *rear = NULL;

    free(temp);
}

void peek(Node *front) {
    if (front == NULL) {
        printf("Queue is empty\n");
        return;
    }
    printf("Front element: %c\n", front->data);
}

void display(Node *front) {
    if (front == NULL) {
        printf("Queue is empty\n");
        return;
    }
    Node *temp = front;
    while (temp != NULL) {
        printf("%c ", temp->data);
        temp = temp->next;
    }
    printf("\n");
}
## Output:

Queue is empty


## Result:
Thus the program was executed and the output was verified successfully.
