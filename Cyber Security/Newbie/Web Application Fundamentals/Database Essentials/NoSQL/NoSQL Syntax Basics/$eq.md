In MongoDB, the `$eq` operator is used to match documents where a specified field is equal to a certain value. It is used in conjunction with the `find` or `update` methods to query or update documents in a collection.

Here is an example of how to use the `$eq` operator:

```
db.collection.find({ field: { $eq: value } })
```

In this example, we're querying a collection for documents where the `field` value is equal to `value`. The `$eq` operator compares the value of the specified field with the given value and returns documents that match the comparison.

The `$eq` operator is often used in combination with other query operators, such as `$lt`, `$lte`, `$gt`, and `$gte`, to perform more complex queries. For example:

```
db.collection.find({ field1: { $eq: value1 }, field2: { $lt: value2 } })
```

In this example, we're querying a collection for documents where the `field1` value is equal to `value1` and the `field2` value is less than `value2`. The `$eq` and `$lt` operators are used together to specify the query criteria.

The `$eq` operator is also the default operator used in MongoDB queries when no operator is specified. For example, the following query is equivalent to the first example:

```
db.collection.find({ field: value })
```

In this example, the `$eq` operator is not explicitly used, but it is assumed by default when no operator is specified.