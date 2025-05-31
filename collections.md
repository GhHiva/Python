The Counter class from Python's collections module is used to count the occurrences of elements in an `iterable` (like a list, string, or tuple). It returns a special dictionary where:

`Keys` are the unique elements in the iterable.

`Values` are the number of times each element appears.

## Common Methods and Features:

| Method or Feature    | Description                                      |                                               |
| -------------------- | ------------------------------------------------ | --------------------------------------------- |
| `most_common(n)`     | Returns the `n` most common elements as a list   |                                               |
| `elements()`         | Returns an iterator over elements (repeats them) |                                               |
| `update(iterable)`   | Adds counts from another iterable or mapping     |                                               |
| `subtract(iterable)` | Subtracts counts (can result in negative values) |                                               |
| `+`, `-`, `&`, \`    | Math operations: combine, subtract, intersect                                             ||
