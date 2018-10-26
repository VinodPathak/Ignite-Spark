Repartition - increase or decrease no of partitions. 
            - Does full shuffle. 
            - Balances data.
            - Slower than Coalesce
            - Preferable(Spark work better with equal size partitions)

Coalesce - decrease no of partitions. 
         - Does partial shuffle(near node data). 
         - Imbalances data across partitions.
         - Faster than Repartition.
