## Background
Automobiles are transported using large trucks which is know as auto-carriers. There are some fixed number of slots that holds the automobiles are known as auto-carrier slots. Automobiles can be of various typoes depending on the size of them. We define three types of automobiles as Type 1 (T1), Type 2 (T2) and Type 3 (T3) that represents small, medium and large automobiles. There are various rules depending on the auto-carrier structure and automobile types that prohibit the automobile assignment to the auto-carrier slots. Those rules are called loading constraints. 
## Loading constraints
There are three type of loading constraints considered in this project. Below the loading costraints are described:
1. Single-car constraint: Certain type of car can not be assigned to certain slots. For Example, T3 automobile can not be assigned to slot 1.
2. Pairwise constraint: If certain type of automobile is assigned to certain slot, some type of automobile can no te assigned to some other slots. For example, If T2 automobile is assigned to slot 1, T3 automobile can not be assigned to slot 2.
3. Multiple space constraint: If some type of automobile is assigned to certain slot it also occupies some other slots. For example, assigning T3 automobile to slot 2 also occupies slot 3.
## What dose this class do?
The LoadingStatesGenerator class takes information about the automobile type, slot ids and the loading constraint to be initialized. The output is a lost of all feasible assignments of automobiles to the auto-carrier slots so that the assignemts do not violate the prohibitions defined by the loading constraints. Each feasible assignment is called loading state. 
## Preparing input
Suppose we have a 3-slot auto-carrier and have three automobiles with automobile id 1, 2 and 3 and their corresponding types are T1, T2 and T3, respectively. The inputs am_types, slot_ids are defined as below:
```python
am_types = {1: "T1", 2: "T2", 3: "T3"}
slot_ids = [1, 2, 3]
```
The three types of constraints are defined for input as follows:
'''
# a list of tuples where each item (t, s) indicates that automobiles of type t can not be assigned to slot s
single_car = [("T3", 1)]
'''
constraints = (single_car, double_slot, pairwise)
