---
title: "Another Python Hiccup"
date: 2022-08-19T12:28:06-04:00
draft: true
---

# The Idea

I generally work through silly pet projects to improve my fluency with a language or data analysis library. This month I've been trying to work through things I already know how to do with `R` and the `tidyverse` and implement them in a `python` script with `pandas`.

## This Week

Here is one thing that I got through this week-- I'm sure this is elementary to some, but if I've learned one thing in statistical programming, it's that if something has annoyed me it's probably also annoyed to someone else.

You can add columns to an index to create a MultiIndex using the `append =` argument in `set_index`.

<p align='left'>

```
df = pd.DataFrame(data = {"Category": [1,1,2,2,2,3,3], 
                          "Cost" : [3.99, 5, 19.54, 20, 23.05, 14, 13.00]}, 
                  index = ['2020-1-12', '2020-1-12', '2020-1-12', '2020-1-12',
                           '2020-1-13', '2020-1-13', '2020-1-13'])

# Append the name of the column that will become an index
df.set_index(keys = ["Category"], append=True, inplace=True)

print(df)

# Use .loc and () to select the rows without having to df["ColumnName"] == value
# The first entry in () uses the first index and the second uses the second.
print(df.loc[("2020-1-12", 2)])
```

</p>

Aaaaand for my next trick, I'll have to figure out how to make sure my code is left aligned in all browsers...
