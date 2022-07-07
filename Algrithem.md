

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

leetcode 206:[Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) (double point/recursion)

Leetcode 160:[Insercion of 2 Link List](https://leetcode.com/problems/intersection-of-two-linked-lists/)

Leetcode 21:[Merge Two](https://leetcode.com/problems/merge-two-sorted-lists/)

Leetcode 86:[Partition List](https://leetcode.com/problems/partition-list/)

Leetcode 142:[Linked List Cycle II and 141 I](https://leetcode.com/problems/linked-list-cycle-ii/)

Leetcode 92:[Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)

#### Stack

Leetcode 20:[Valid Parentheses](https://leetcode.com/problems/valid-parentheses/)(dic, stack = ['?'] 占一个位置)

Leetcode 244:[Basic Calculator](https://leetcode.com/problems/basic-calculator/)

Leetcode 155:[Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)

Leetcode 946:[Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)

Leetcode 793:[Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)

Leetcode 142:[Linked List Cycle II](https://leetcode.com/problems/linked-list-cycle-ii/)

#### Queue

Circular queue, double-ended queue, priority queue

Leetcode 232:[Implement Queue using Stacks](https://leetcode.com/problems/implement-queue-using-stacks/)

heap的应用(priority queue) __找最大值最小值__

堆：binary tree, 小根堆：every parent node <= each of its children. 大根堆相反. 
所以小根堆的最小元素是__heap[0]__

```python 
heap[k] <= heap[2*k+1] and heap[k] <= heap[2*k+2]
```

​					0
​				1		2
​			 /	 \	/    \
​		   3	  4  5	  6

```python
# python 默认是小根堆
import heapq
heapq.heapify(list) # 在linear time内把list转化成 heap
heapq.heappush(heap,x) # 插入到堆中，并且保持堆的特性不变
heapq.heappop(heap) # 弹出最小值，并保持堆特性不变，如果heap为空，抛出异常，heap[0] 取最小元素
heapq.heappushpop(heap,x) # 弹出最小元素，并把x push进堆中
heapq.heapreplace(heap,item) # 弹出最小元素，并用item替代 和heappushpop()差不多
    nums = [6,4,3,2,1,0]
    heapq.heapify(nums)
    nums
    output：[0, 1, 3, 2, 4, 6]
    heapq.heapreplace(nums,10)
    output：[1, 2, 3, 10, 4, 6]
heap.nlargest(n,iter,key=None)
heap.nsmallest(n,iter,key=None) # 返回iter中最小的n个元素的list
heap.mearge(*iterables,key=None,reverse=None) #合并两个heap
```

Leetcode 239[Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum/)(用到了heap知识)



|          | Stack                                   | Queue                            |
| -------- | --------------------------------------- | -------------------------------- |
|          | LIFO                                    | FIFO                             |
| Insert   | Push()                                  | Enqueue()                        |
| Deletion | Pop()                                   | Dequeue()                        |
|          | One point used for perfroming operation | 2 points uset for opreation      |
| Full？   | Top == MAX-1                            | Frount == -1 or Front == rear +1 |
| Empty？  | Top == -1                               | Rear == MAX-1                    |
| Solve    | Recursing Quiz                          | Sequential Quiz                  |





