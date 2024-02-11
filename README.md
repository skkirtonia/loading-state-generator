## Background
Automobiles are transported using large trucks which is know as auto-carriers. There are some fixed number of slots that holds the automobiles are known as auto-carrier slots. Automobiles can be of various typoes depending on the size of them. We define three types of automobiles as Type 1 (T1), Type 2 (T2) and Type 3 (T3) that represents small, medium and large automobiles. There are various rules depending on the auto-carrier structure and automobile types that prohibit the automobile assignment to the auto-carrier slots. Those rules are called loading constraints. 
## Loading constraints
There are three type of loading constraints considered in this project. Below the loading costraints are described:
1. Single-car constraint: Certain type of car can not be assigned to certain slots. For Example, T3 automobile can not be assigned to slot 1.
2. Pairwise constraint: If certain type of automobile is assigned to certain slot, some type of automobile can no te assigned to some other slots. For example, If T2 automobile is assigned to slot 1, T3 automobile can not be assigned to slot 2.
3. Multiple space constraint: If some type of automobile is assigned to certain slot it also occupies some other slots. For example, assigning T3 automobile to slot 2 also occupies slot 3.
