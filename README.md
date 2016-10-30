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


Project Team
==============
* Ankur Patel
* GuruPrasad 
* Vignesh Ramesh
