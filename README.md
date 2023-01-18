# My Python Guidelines

## Style guidelines

Based on [PEP8](https://peps.python.org/pep-0008/).

### pylint

Use [pylint](https://pylint.pycqa.org/en/latest/) to validate these style guidelines.

*TODO*

### Code Lay-out

* **4 spaces indentation**

```python
# Aligned with opening delimiter.
foo = long_function_name(var_one, var_two,
                         var_three, var_four)

# Add 4 spaces (an extra level of indentation) to distinguish arguments from the rest.
def long_function_name(
        var_one, var_two, var_three,
        var_four):
    print(var_one)

# Hanging indents should add a level.
foo = long_function_name(
    var_one, var_two,
    var_three, var_four)
    
# No extra indentation.
if (this_is_one_thing and
    that_is_another_thing):
    do_something()

# Add a comment, which will provide some distinction in editors
# supporting syntax highlighting.
if (this_is_one_thing and
    that_is_another_thing):
    # Since both conditions are true, we can frobnicate.
    do_something()
 
my_list = [
    1, 2, 3,
    4, 5, 6,
    ]
result = some_function_that_takes_arguments(
    'a', 'b', 'c',
    'd', 'e', 'f',
    ) 
```

* **maximum line length 79 characters ?**

* **line break before binary operator**

```python
# easy to match operators with operands
income = (gross_wages
          + taxable_interest
          + (dividends - qualified_dividends)
          - ira_deduction
          - student_loan_interest)
```

* **blank lines**

  * Surround top-level function and class definitions with two blank lines.

  * Method definitions inside a class are surrounded by a single blank line.

  * Extra blank lines may be used (sparingly) to separate groups of related functions. Blank lines may be omitted between a bunch of related one-liners (e.g. a set of dummy implementations).

  * Use blank lines in functions, sparingly, to indicate logical sections.
  
* **source file encoding**

always use UTF-8

??? and should not have an encoding declaration ?

all identifiers use ASCII-only identifiers and use English words

* **imports**

*TODO*

## Documentation guidelines

Based on [PEPE257](https://peps.python.org/pep-0257/).

*TODO*

## Docker packaging guildelines

*TODO : based on python3 images *
