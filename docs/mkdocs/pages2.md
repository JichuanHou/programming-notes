# Page 2

## Another Heading

Some more example text


## Code Annotation Examples

### Code blocks

Some `code` goes here

### Plain codeblock

A plain codeblock

```
Some code here
def myfunction()
// some comment
```

### Code for a specific language

Some more code with the 'py' at the start;

``` py
import tensorflow as tf
def whatever()
```

### Code with a title

``` py title="bubble_sort.py"
def bubble_sort(items):

```

``` py linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items)-1-i):
            if items[j] > items[j+1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

``` py hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items)-1-i):
            if items[j] > items[j+1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Icons and Emojis

:smile:

:fontawesome-regular-face-laugh-wink:

:fontawesome-brands-twitter:{ .twitter }

:octicons-heart-fill-24:{ .heart }