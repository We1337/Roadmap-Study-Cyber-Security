In MongoDB, the `$ne` operator is used to query for documents where a specified field is not equal to a certain value. It is used in conjunction with the `find` method to retrieve documents from a collection that do not match a specific value.

Here is an example of how to use the `$ne` operator:

```
db.collection.find({ field: { $ne: value } })
```

In this example, we're querying a collection for documents where the `field` value is not equal to `value`. The `$ne` operator compares the value of the specified field with the given value and returns documents that do not match the comparison.

The `$ne` operator can also be used in combination with other query operators, such as `$lt`, `$lte`, `$gt`, and `$gte`, to perform more complex queries. For example:

```
db.collection.find({ field1: { $ne: value1 }, field2: { $lt: value2 } })
```

In this example, we're querying a collection for documents where the `field1` value is not equal to `value1` and the `field2` value is less than `value2`. The `$ne` and `$lt` operators are used together to specify the query criteria.

Note that the `$ne` operator can impact query performance, especially on large collections, as it requires a full scan of the collection. In general, it's recommended to use `$eq` or other query operators whenever possible, and only use `$ne` when you need to exclude a specific value from the query results.