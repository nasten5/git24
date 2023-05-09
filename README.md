HomeWork6
mport java.util.LinkedList;
import java.util.PriorityQueue;
import java.util.Queue;

public class PriorityQueueExample {
public static void main(String[] args) {

Queue<Integer> queueL = new LinkedList<>();
for (int i = 5; i > 0; i--) {
queueL.add(i);
}
System.out.println("Print our LinkedList Queue (FIFO): " + queueL);
Queue<Integer> priorityQueue = new PriorityQueue<>();

for (int i = 5; i > 0; i--) {
priorityQueue.offer(i);
}

System.out.println("PriorityQueue printing (by iterating, no elements removing): " + priorityQueue);
System.out.println("Print PriorityQueue using poll() (by retrieval): " );
while (!priorityQueue.isEmpty()) {
System.out.println(priorityQueue.poll());
}
}
}
Print our LinkedList Queue (FIFO): [5, 4, 3, 2, 1]
PriorityQueue printing (by iterating, no elements removing): [1, 2, 4, 5, 3]
Print our PriorityQueue using poll() (by retrieval):
1
2
3
4
5
