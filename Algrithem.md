### 链表，栈，队列

#### 单链表，双链表，循环链表

单链表

![ZRJVrq](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021148165.png)

![ZRJVrq](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021148984.png)

双链表，循环链表

![vuUVJn](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021149956.png)

data：可以是任意数据结构 
nest/pre：指向前后的指针.

```c
typedef struct Node{
  int data;
  struct Node *next
}Node, *LinkedList;
```

