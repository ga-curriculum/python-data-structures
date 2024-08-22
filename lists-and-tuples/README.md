<h1>
  <span class="headline">Python Data Structures</span>
  <span class="subhead">Lists and Tuples</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand and utilize different data structures in Python, including lists, tuples, and sets, for managing and manipulating collections of data.

| Lesson           | Duration |
| ---------------- | -------- |
| Lists and Tuples | 40 min   |

## Lists

A **list** is an ordered collection of data combined into one variable. Each item in a list is assigned an **index** value based on its position. These index values allow us to access individual elements within the list.

```python
["banana", "orange", "apple"]
    0         1         2
```

<!-- ![Image Placeholder](TKTK) -->

## Syntax

You create a list using a set of square brackets. Inside the brackets, each value must be separated by a comma. Although it most often makes sense for all values to be the same data type, there’s no rule against using a list to store data of varying types.

```python
fruits = ["banana", "orange", "apple"]
```

## Accessing List Values

```python
fruits = ["banana", "orange", "apple"]

# fruits[0] will access "banana"

# fruits[1] will access "orange"

# fruits[2] will access "apple"

```

> Access list items using square brackets around their index values. It’s pretty simple — just remember that the first index value is always zero!

## Updating List Values

We can update the items in a list using the same index syntax. The same assignment operator that we used with individual variables can also be used to set the value of a specific item in a list.

```python
fruits = ["banana", "orange", "apple"]
fruits[0] = "kiwi"
fruits[1] = "strawberry"

# The fruits list now looks like ["kiwi", "strawberry", "apple"]
```

<br>

<div class="activity solo-exercise">
  <h2 class="title">2.1 Colors of the Rainbow</h2>
  <span class="minutes">15 min</span>
</div>

Let’s practice creating a list, along with accessing and updating values using the specific list index syntax.

<!-- ![Image Placeholder](TKTK) -->

## List Methods

In addition to using index syntax to refer to specific items, we can also use **methods** of lists to perform specific actions on that list. The syntax looks like:

```python
list_name.method_name( any_inputs_here )
```

The parentheses might remind you of the print statements we’ve used thus far. That’s because, just like `print()`, methods can also accept specific input, or **arguments**, for their operations.

## Adding Items with `.append()`

The `.append()` method **adds** the item inside the parentheses to the **end** of the list.

```python
fruits = ["orange"]
fruits.append("kiwi")

# fruits is now: ["orange", "kiwi"]
```

## Adding Items with `.insert()`

The `.insert()` method starts by taking an index number, then **adds** the second argument in the parentheses to the given index. Note the original item at that index is simply bumped to the next spot in the list.

```python
fruits = ["orange", "kiwi"]
fruits.insert(1, "lemon")

# fruits is now: ["orange", "lemon", "kiwi"]
```

## Removing Items with `.pop()`

The `.pop()` method can be used to **remove** the item at a specific index, or, if you don’t provide any index, it will simply remove the last item in the list.

```python
fruits = ["orange", "kiwi", "lime"]
fruits.pop()

# fruits is now: ["orange", "kiwi"]

fruits.pop(0)

# fruits is now: ["kiwi"]
```

<br>

<div class="activity partner-exercise">
  <h2 class="title">2.2 The Wait List</h2>
  <span class="minutes">20 min</span>
</div>

Let’s practice these list methods and more by managing the waiting list for the Python Academy, the most exclusive private boarding school in all of East Python-shire.

<!-- ![Image Placeholder](TKTK) -->

## More List Functions

| **Function**        | **Explanation**                                  | **Example**                                                                                 |
| ------------------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------- |
| `len()`             | Produces the length of the list.                 | `python fruits = ["apples", "bananas", "oranges"]`<br> `len(fruits)`<br> `# 3`              |
| `min()` and `max()` | Produces the minimum or maximum.                 | `python scores = [10, 20, 30]`<br> `min(scores)` <br> `# 10` <br> `max(scores)` <br> `# 30` |
| `sum()`             | Produces the total sum of all items in the list. | `python sales = [25, 15, 10]` <br> `sum(sales)` <br> `# 50`                                 |

> 💡 This is simply to show that not all functions involving lists have to be methods of the list itself. Some of these aggregate functions will be very important for the purposes of analysis, and no discussion of lists is complete without introducing `len()`.

## Tuples: You Already Know Them!

The good news about `tuples` is that they work exactly the same way as lists, but simply use parentheses instead of square brackets.

```python
valid_statuses = ("operational", "faulty", "non-operational")
```

The difference is that tuple values are **_immutable_**, meaning you cannot change values in a tuple once it’s been created; thus, tuples are mostly used for reference information that will not change.

## Sets

A **set** is an unordered collection of unique values. You can’t use an index to access a specific element in a set. Instead, sets have methods for accessing or manipulating collection members:

```python
primary_colors = { "red", "blue", "yellow" }
primary_colors.add("green")
primary_colors.remove("yellow")
```
