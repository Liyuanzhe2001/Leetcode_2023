# Leetcode_2023

PriorityQueue<>  优先队列 小顶堆
Queue<Integer> bigHeap = new PriorityQueue<>((x,y) -> y - x); 大顶堆
```text
add(E e) - 向优先队列中插入元素，插入失败抛出异常
offer(E e) - 向优先队列中插入元素，插入失败返回false 
element() - 获取但不删除队首元素，获取失败抛出异常
peek() - 获取但不删除队首元素，获取失败返回null
remove() - 获取并删除队首元素，失败时抛出异常
poll() - 获取并删除队首元素，失败时返回null
remove(Object o) - 删除队列中跟o相等的某一个元素（如果有多个相等，只删除一个）
```

辗转相除法求最大公约数
```text
public int gcd(int a, int b) {
    while (b != 0) {
        int temp = a;
        a = b;
        b = temp % b;
    }
    return a;
}
```

裴蜀定理
```text
裴蜀定理（或贝祖定理）说明了对任何整数a、b和它们的最大公约数d，关于未知数x和y的线性不定方程（称为裴蜀等式）：若a,b是整数,且gcd(a,b)=d，那么对于任意的整数x,y,ax+by都一定是d的倍数，特别地，一定存在整数x,y，使ax+by=d成立。
它的一个重要推论是：a,b互质的充分必要条件是存在整数x,y使ax+by=1.
```

单个键值对
```text
AbstractMap.SimpleEntry<String, Integer> key = new AbstractMap.SimpleEntry<>("key", 9527);
```
