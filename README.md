# Distributed-Key-Value-Store
Distributed System - Course Project

Developed an in memory key-value store (Distributed Systems course project) with features like
* Detection of Strict Consistency or Eventually consistent
* Support for Consistency levels


Requirements
=======
* Apache Thrift
* Java 1.7

API Documentation
=======
##key-value Store

1) Get  - If a key-value pair exists, return its value and kSuccess. If a key-value pair does not exist, return error kKeyNotFound.
```bash
./kvclient -server host:port -get 'my_key' > my_value_file
```

2) Set - If a key-value pair already exists, overwrite its value. If a key-value pair does not already exist, create it.
```bash
./kvclient -server host:port -set 'my_key' 'my_value'
```

3) Del - If a key-value pair exists, delete it and return kSuccess. If a key-value pair does not exist, return kKeyNotFound.
```bash
./kvclient -server host:port -del 'my_key'
```
##Consistency Check

1) To compile all the java files, run the script Compile_all.
```bash
  $ ./compile_all
```
2) To run the sequence server, run the script SequenceServer. This will run on the port 5432.
```bash
  $ ./sequence_server
```
3) To run the KVClient, run the script

* If the server is consistent

```bash
  $ ./consistency_test -server 192.168.1.5:9634
  $ echo $?
  0
```
* If the server is Inconsistent
```bash
  $ ./consistency_test -server 192.168.1.5:9634
  $ echo $?
  1
```
* If the test is inconclusive (e.g., the server stopped responding)
```bash
  $ ./consistency_test -server 192.168.1.5:9634
  $ echo $?
  2
```

Project Team
==============
* Ankur Patel
* GuruPrasad
* Vignesh Ramesh
