# Distributed-Key-Value-Store
Distributed System - Course Project

Developed an in memory key-value store (Distributed Systems course project) with features like 
* Detection of Strict Consistency or Eventually consistent
* Support for Consistency levels

API Documentation
=======
1) Set  - If a key-value pair already exists, overwrite its value. If a key-value pair does not already exist, create it. 
```bash 
Result kvset(1:string key, 2:string value)
```


   // If a key-value pair already exists, overwrite its value.
   // If a key-value pair does not already exist, create it.
   ,

   // If a key-value pair exists, return its value and kSuccess.
   // If a key-value pair does not exist, return error kKeyNotFound.
   Result kvget(1:string key),


   // If a key-value pair exists, delete it and return kSuccess.
   // If a key-value pair does not exist, return kKeyNotFound.
   Result kvdelete(1:string key),


Project Team
==============
* Ankur Patel
* GuruPrasad 
* Vignesh Ramesh
