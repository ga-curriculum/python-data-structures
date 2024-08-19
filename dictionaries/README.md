<h1>
  <span class="headline">Python Data Structures</span>
  <span class="subhead">Dictionaries</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to define and use dictionaries in Python, including creating, accessing, and updating key-value pairs.

| Lesson       | Duration |
| ------------ | -------- |
| Dictionaries | 25 min   |

## Dictionary Definition

A dictionary is a collection of associated **keys** and **values**. Think of a dictionary like a row of data in a spreadsheet — you have column names, which are your keys, and then you have the actual values inside of the columns.

| item_name | category | price |
| --------- | -------- | ----- |
| tomatoes  | food     | 1.99  |

The above row would be translated into this dictionary:

```python
{ "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

## Syntax for Dictionaries

```python
item = { "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

![Image Placeholder](TKTK)

Curly braces are used to start and end the dictionary.

```python
item = { "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

![Image Placeholder](TKTK)

Key names are provided first and surrounded by quotation marks.

```python
item = { "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

![Image Placeholder](TKTK)

Values are provided after a colon and can be of any data type.

```python
item = { "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

![Image Placeholder](TKTK)

Finally, note the commas separating each key-value pair.

## Accessing Values in a Dictionary

```python
item = { "item_name": "tomatoes", "category": "food", "price": 1.99 }
```

Accessing specific values in a dictionary works a lot like accessing specific items in a list. This time, instead of numbered indices, we use the name of the key.

```python
item["category"]

# This accesses the value "food"
```

## Adding Values to a Dictionary

One of the most powerful features of a dictionary is the ability to add new keys and values whenever necessary.

```python
item["fresh"] = True
item["discount"] = .15
```

The same syntax can update a given property as well.

```python
item["fresh"] = False
```

<br>

<div class="activity solo-exercise">
  <h2 class="title">2.3 Key Value Properties</h2>
  <span class="minutes">15 min</span>
</div>

Practice accessing and updating properties in a dictionary by modifying a real estate listing in **Section 2.3** of the Jupyter Notebook.

## Representing a Data Set

<br>

<div class="activity knowledge-check">
  <h2 class="title">Representing a Data Set</h2>
  <span class="minutes"></span>
</div>

Based on what we know about data structures, **how would we represent an entire data set (like a .csv file)**, with many rows and columns of information, **in Python**?

| item_name | category | price |
| --------- | -------- | ----- |
| tomatoes  | food     | 1.99  |
| mango     | food     | 3.00  |
| journal   | office   | 15.00 |


<details>
<summary>✅ Click to see the answer: </summary>
<hr>

A List of Dictionaries!

Each dictionary is a specific row, and the list is our "table" collecting all of the rows together.

<hr>
</details>

<br>

> 💡 Hopefully this connection to data formats the students are already familiar with helps solidify the role of lists and dictionaries in data analysis. Dictionaries can be tricky to understand, so the comparison to rows and columns can help familiarize the concept.
