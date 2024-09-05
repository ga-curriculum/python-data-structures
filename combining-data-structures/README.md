<h1>
  <span class="headline">Python Data Structures</span>
  <span class="subhead">Combining Data Structures</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand and navigate nested data structures by accessing values at various levels of complexity.

| Lesson                    | Duration |
| ------------------------- | -------- |
| Combining Data Structures | 25 min   |

## Nested Data Structures

So far, we’ve seen lists and dictionaries that organize simpler data types, like strings and numbers. However, it’s common to see the more complex data structures nested within each other, creating elaborate mazes of data.

When getting data from outside sources, for example, you might be given a dictionary that contains another dictionary that contains a list containing another dictionary that **finally** contains the information you’re looking for!

> 💡 Nested data structures can make programming complicated, but they are also what makes it more powerful than other analysis tools like Excel.
>
> - You can’t have a cell that’s actually an entire table, but you can have a dictionary that contains another list of dictionaries, and so on.
> - This ability to build in powerful, complex relationships between data is a compelling benefit of Python over more user-friendly data analysis tools.

<br>

<div class="activity discussion">
  <h2 class="title">What Is This Accessing?</h2>
  <span class="minutes"></span>
</div>

Think about what the following line of code is saying, one layer at a time:

```python
authors[0]["books"][1]["title"]
```

_Without seeing the exact data structure in question, what is this line attempting to access?_

<br>

<div class="activity discussion">
  <h2 class="title">Peeling Back the Layers</h2>
  <span class="minutes"></span>
</div>

_What does each layer do?_

```python
authors[0]

# There is a list called authors and we want the first thing in it.
```

```python
authors[0]["books"]

# There is a list called authors and we want the first thing in it.

# That first thing is a dictionary and we want the "books" property.
```

```python
authors[0]["books"][1]

# There is a list called authors and we want the first thing in it.

# That first thing is a dictionary and we want the "books" property.

# Turns out "books" is a list and we want the second thing in it.
```

```python
authors[0]["books"][1]["title"]

# There is a list called authors and we want the first thing in it.

# That first thing is a dictionary and we want the "books" property.

# Turns out "books" is a list and we want the second thing in it.

# That second thing is another dictionary with a "title" property.
```

## Keep Calm and `print()` On

When dealing with a complex, multi-level data structure, you can lean on print statements to help peel back the layers one at a time. The syntax for accessing elements doesn’t change, you just simply need more layers:

```python
print(authors[0])
print(authors[0]["books"])
print(authors[0]["books"][1])
print(authors[0]["books"][1]["title"])
```

> 💡 You can demonstrate this process using the notebook challenge’s complex data structure to illustrate the point.
> You can also add more properties/nested structures to repeat the technique.

<br>

<div class="activity partner-exercise">
  <h2 class="title">2.4 Python Librarian</h2>
  <span class="minutes">15 min</span>
</div>

Managing nested data structures can be difficult!
Work through the challenges of accessing and modifying the "authors" dictionary found in **Section 2.4** of the workbook.

<img src="./assets/open-book.png" alt="Open Book Image" style="width: 300px; height: auto;">

_If you aren't able to finish this in class, we encourage you to complete it as homework for more practice._
