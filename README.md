**🧾 Project Overview**

This project performs frequent itemset mining on a traffic-related dataset using two classical algorithms: Apriori and FP-Growth. The objective is to analyze the efficiency and performance of these algorithms in terms of:
1.Time complexity
2.Number of frequent patterns found
3.Support values across iterations
The focus is on identifying frequent co-occurring events, such as traffic congestion signals (SGN1), traffic flow (T), and priority routes (PR1), and evaluating how well each algorithm handles large datasets.


**🔍 Dataset Details**

The dataset comprises transactional-style records representing traffic patterns. Each record consists of multiple items such as:
1. T: Traffic event
2. SGN1: Signal 1 active
3. PR1, SC3: Priority route or sensor check active
_Support Thresholds:_

_**1.First Iteration: Minimum support = 0.4
2.Subsequent Iterations: Minimum support = 0.1**_

**🧠 Algorithms Used**

_🔶 Apriori_
1. Classical breadth-first algorithm
2. Candidate generation + pruning
3. Runtime: ~1.0002 seconds
_🔷 FP-Growth_
1. Tree-based depth-first approach
2. Avoids candidate generation
3. Runtime: ~0.4715 seconds
   
**📈 Top 10 Frequent Itemsets**
_Apriori:_
Found itemsets like: (T), (SGN1), (T, SGN1), (PR1), (T, SGN1, PR1)
Slower due to multiple passes and candidate generation
_FP-Growth:_
Identified same top itemsets
More efficient with ~50% reduction in runtime

