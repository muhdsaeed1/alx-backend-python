An async comprehension is an asynchronous version of a classical comprehension.

Asyncio supports two types of asynchronous comprehensions, they are the “async for” comprehension and the “await” comprehension.

Comprehensions
Comprehensions allow data collections like lists, dicts, and sets to be created in a concise way.

A list comprehension allows a list to be created from a for expression within the new list expression.

For example:

...
# create a list using a list comprehension
result = [a*2 for a in range(100)]
Comprehensions are also supported for creating dicts and sets.

For example:

...
# create a dict using a comprehension
result = {a:i for a,i in zip(['a','b','c'],range(3))}
# create a set using a comprehension
result = {a for a in [1, 2, 3, 2, 3, 1, 5, 4]}

Asynchronous Comprehensions
An asynchronous comprehension allows a list, set, or dict to be created using the “async for” expression with an asynchronous iterable.


...
# async list comprehension with an async iterator
result = [a async for a in aiterable]
This will create and schedule coroutines or tasks as needed and yield their results into a list.

Recall that the “async for” expression may only be used within coroutines and tasks.



