### 链表，栈，队列

#### 单链表，双链表，循环链表

单链表

![ZRJVrq](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021148165.png)

![ZRJVrq](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021148984.png)

data：可以是任意数据结构 
pre：指向后的指针.
链表的创建，初始化，插入（头插，尾插），遍历，删除

双链表
	前后两个指针next/pre, 一定要同时指向，第一个和最后一个指向NULL

循环链表

![vuUVJn](https://raw.githubusercontent.com/lixiang7610/Machine-learning-Revision/main/img/202207021149956.png)

leetcode 206:[Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/)
Leetcode 160:[Insercion of 2 Link List](https://leetcode.com/problems/intersection-of-two-linked-lists/)
Leetcode 21:[Merge Two](https://leetcode.com/problems/merge-two-sorted-lists/)
Leetcode 86:[Partition List](https://leetcode.com/problems/partition-list/)
Leetcode 142:[Linked List Cycle II and 141 I](https://leetcode.com/problems/linked-list-cycle-ii/)
Leetcode 92:[Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)

#### Stack

#### Queue

Circular queue, double-ended queue, priority queue

|          | Stack                                   | Queue                            |
| -------- | --------------------------------------- | -------------------------------- |
|          | LIFO                                    | FIFO                             |
| Insert   | Push()                                  | Enqueue()                        |
| Deletion | Pop()                                   | Dequeue()                        |
|          | One point used for perfroming operation | 2 points uset for opreation      |
| Full？   | Top == MAX-1                            | Frount == -1 or Front == rear +1 |
| Empty？  | Top == -1                               | Rear == MAX-1                    |
| Solve    | Recursing Quiz                          | Sequential Quiz                  |





