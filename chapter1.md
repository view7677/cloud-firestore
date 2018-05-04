# About Cloud Firestore

Cloud firestore is a NoSQL, document-oriented database similar to Mongo database. Data are stored in _documents_, which are organized into _collections_.


A _document_ contains a set of key-value pair. A _document_  can contain _subcollections_ and nexted objects.

Collections and documents are created implicity in Cloud Firestore. 


## Documents

A document is a record of key-value.key is the field name, Value is Value map to the key. You can think similar to JSON object but not exactly.

A document represetning a user `vijay` look like this.

```json
    vijay:
        name:
            first:"Vijay",
            last:"Keshri"
        born: 1979
```
Diffence between a _document_ and a JSON object is , document support extra datatype and are limited in size to 1 MB.

## Collections

A _collections_ has one or more _document_ . For example `users` collection.


```json

users:
    vijay:
        name:
            first:"Vijay",
            last:"Keshri"
        born: 1979
    ajay:
        name:
            first:"Ajay",
            last:"Gupta"
        born: 1978
```

a _collection_ can't exist without a _document_. If you delete all the _documents_ from a _collection_, _collection_ would be deleted.


## References