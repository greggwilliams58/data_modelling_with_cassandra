# data_modelling_with_cassandra
This is part of the Udacity "Data Engineering course".  The purpose of this exercise was to demonstrate some basic data modelling required to work with NoSQL databases.  That is chiefly to build primary keys based on both fields used in the WHERE clause and to establish a unique row identifer within the dataset.

##Task of the code##
The code within the notebook is split into two parts

1. __For pre-processing of the source data__
importing the required python packages, establishing the end user's folder path structure, create a list of lists which is then inserted into the "event_datafile_full" csv file.

2. __Writing the queries__
This is a series of tasks.
    1. Create a Cassandra Cluster
    2. Create a Keyspace
    3. For each query the following sequence is followed
        1. Define and create the table
        2. Insert values from the CSV file into the table
        3. Define and execute the query
        4. Print results set to the console and conver to a pandas dataframe
    4. Drop the table
    5. Close the session and cluster.
