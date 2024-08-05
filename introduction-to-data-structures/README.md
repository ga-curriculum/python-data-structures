<h1>
  <span class="headline">Python Data Structures</span>
  <span class="subhead">Introduction to Data Structures</span>
</h1>

**Learning objective:** By the end of this section, learners will be able to identify and apply the appropriate data structure—list, tuple, or dictionary—for organizing and managing data in Python.

| Lesson                          | Duration |
| ------------------------------- | -------- |
| Introduction to Data Structures | 15 min   |

## Our Learning Goals

- Use lists and list methods to manage collections of data.
- Use index-based retrieval to access and manipulate list items.
- Use dictionaries to represent data with multiple properties.

## What We’ll Practice

This Module connects to and reinforces topics that you encountered in the pre-work.
We’re going to return to topics covered in the pre-work and build upon them:

- Data structures like lists, tuples, and dictionaries.
- Combining data structures.
- List methods.

## Solo Exercise : Jupyter Notebook (10 min) tktk

Let’s dive right in and use what we learned in the pre-work! We want to understand where you are in your learning journey so that we can give the best possible experience in class.

- Look over the exercises in today's Jupyter Notebook and attempt any that seem immediately doable to you.
- Then, rate your confidence level on today's subjects from 1–5.

## Our Sad, Unstructured Data

So far, our variables have only stored a single piece of information, or data. Imagine trying to represent a data set using this method:

```python
customer_one = "Anees Rosario"
customer_two = "Alya Pham"
customer_three = "Marc Wormald"
customer_four = "Ellie-Mai Muir"
```

You won’t get very far using a new variable for every new piece of data!

> 🍎 Note also how "hard-coded" this list would be — you would have to remember exactly which variable contained each string!
> And what happens when we want to get rid of "customer_three" and move everyone else up by one?

## Data Structures to the Rescue!

Fortunately, Python provides us with some options for compiling data into a single structure:

- **Lists** - are exactly what they sound like: comma-separated lists of values.
- **Tuples** - are like lists but more strict. You can’t update the values in a tuple!
- **Dictionaries** - allow us to associate multiple properties together, much like a single row of a spreadsheet can contain many columns.

## Discussion : Guess the Data Structure! tktk

Before we get into the specifics, let’s think about which of our three data structures (lists, tuples, and dictionaries) makes the most sense when representing the following information:

- The five continents on Earth.
- An item for sale in our store.
- All transactions conducted in our store.
- A single transaction conducted in our store.
- A weather forecast for today.
- The three possible quality rankings for produce.

## Data Structures Revealed

Tuples hold values that will not change, while lists can be updated more easily. Dictionaries represent a single, but complex, piece of information.

<details>
<summary>✅ Click to see the answer: </summary>
<hr>

- The five continents on Earth: `Tuple`.

- An item for sale in our store: `Dictionary`.

- All transactions conducted in our store: `List`.

- A single transaction conducted in our store: `Dictionary`.

- A weather forecast for today: `Dictionary`.

- The three possible quality rankings for produce: `Tuple`.

<hr>
</details>

<br>

> 🍎 The common theme here is that tuples hold values that will not change over time. You might have to update a transaction, but reference data such as continents or quality ranks won’t change. Dictionaries represent a single, but complex piece, of information with multiple properties.
