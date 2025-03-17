# SQPM-Lab4

Introduction:
This report documents the implementation and evaluation of inter-process communication (IPC) methods using shared memory and message queues in a Linux environment. The goal of this lab is to explore how different processes can exchange data efficiently and to compare the advantages and limitations of these IPC mechanisms. Effective communication between processes is essential in many real-world applications, including operating systems, networking, and concurrent programming. The tasks in this lab involve implementing shared memory using system calls such as shmget and shmat, which allow multiple processes to access the same memory segment. Additionally, message queues are implemented using msgsnd and msgrcv, which enable structured message-passing between processes. By working with these IPC methods, we analyze key factors such as data synchronization, consistency, memory management, and performance trade-offs. Through this lab, we gain hands-on experience with IPC concepts and develop a better understanding of how operating systems handle process communication. By comparing shared memory and message queues, we can determine which method is more efficient for different use cases and discuss potential challenges such as race conditions and access control. The insights from this lab will help in understanding concurrent programming techniques and optimizing process interactions in larger systems.

Discussion:

Accuracy represents the proportion of correct predictions—both true positives and true negatives—out of all predictions made. It provides a general measure of a model’s effectiveness. In cases where the dataset is evenly distributed between positive and negative instances, a high accuracy score suggests reliable model performance. However, accuracy can be deceptive in scenarios involving imbalanced datasets. For instance, if 95% of emails in a dataset are non-spam, a model that always predicts "non-spam" would still achieve 95% accuracy, despite completely failing to identify spam emails.

Recall, also known as sensitivity, quantifies the percentage of actual positive cases that the model correctly detects. It is calculated using the formula:

Recall=TP/(TP+FN)

This metric is particularly crucial in situations where missing a positive case could have serious consequences. A prime example is medical diagnostics—if a model is used to detect a life-threatening disease, a high recall ensures that most actual cases are identified. Even if it means increasing false positives, reducing false negatives is more critical for patient safety.
Precision measures the accuracy of positive predictions, ensuring that when a model classifies an instance as positive, it is likely correct. It is given by:

Precision=TP/(TP+FP)

Precision is especially valuable in cases where false positives are costly. A good example is email spam filtering. If a spam filter incorrectly labels important emails as spam, the user might miss crucial information. Therefore, optimizing for high precision ensures that flagged emails are highly likely to be actual spam.

Applications Where Different Metrics Take Priority

Recall-Oriented Applications: In critical fields such as cancer screening, maximizing recall is essential. The goal is to identify all potential cases of cancer, even if it means flagging some non-cancerous cases incorrectly. Missing an actual case (false negative) could have severe consequences, making recall the priority over precision.

Precision-Oriented Applications: In contrast, applications such as spam detection prioritize precision. Users prefer to occasionally receive spam (lower recall) rather than risk losing important emails due to false positives. Thus, a spam filter should aim for high precision to ensure that only actual spam is flagged.

Balanced Metrics (Accuracy-Focused Applications): When both classes are equally significant and the cost of errors is comparable, accuracy can serve as a reliable performance measure. For instance, in manufacturing quality control, where defects are uncommon but crucial to detect, accuracy provides a broad assessment of performance when analyzed alongside recall and precision.

Conclusion:

This lab provided hands-on experience with inter-process communication (IPC) using shared memory and message queues in a Linux environment. By implementing and analyzing these methods, we gained insight into their efficiency, synchronization challenges, and real-world applications. Shared memory allows fast data exchange but requires careful synchronization to prevent race conditions. It is ideal for high-speed applications but demands additional complexity in managing concurrent access. In contrast, message queues offer structured, asynchronous communication with built-in synchronization but introduce processing overhead due to message copying. While shared memory is optimal for speed, message queues are more reliable for ordered communication. Through this lab, we reinforced key concepts in concurrency, synchronization, and process interaction. Understanding these IPC mechanisms helps in designing efficient software systems, making informed decisions about communication strategies, and optimizing performance in real-world applications.

Screenshots taken throughout this lab:

Screenshot 1:


Screenshot 2:


Screenshot 3:


