# Test Suites

This repository contains the test suites as described in the paper:

[Searching for Better Database Queries in the Outputs of Semantic Parsers](https://arxiv.org/pdf/2210.07201.pdf)

## Data

The test suites can be downloaded from [this link](https://drive.google.com/drive/folders/1K5PzF6hxXsjw1Y44pkBj222c4rvtVtxb?usp=share_link).

The test suites were created for five datasets: Spider, GeoQuery, IMDB, Yelp, and Academic.

The names of the database files for each dataset are in the following format:

```{dataset_name}_{test_database_count}_{gold_query_index}_ts.sqlite```

The ```gold_query_index``` is the index of the corresponding gold query. You can find the mapping between the gold queries and their indexes in the file ```{dataset_name}_query_to_index.json```, which is located in each dataset folder.

For each gold query, there is a separate test suite with several test databases. The ```test_database_count``` parameter enumerates all the databases corresponding to a given gold query. For instance, if a gold query in the Yelp dataset has an index of ```gold_query_index=5```, there would be three test databases in the test suite, named ```yelp_0_5_ts.sqlit```, ```yelp_1_5_ts.sqlite```, and ```yelp_2_5_ts.sqlite```.
