### In Local mode:
* if data is large then number of partitions is dataset_size/128
* if dataset is small then number of partitions is dataset_size/num_of_threads(i.e. master local[8], here it is 8)
