# Drink about (Python solution)

## Instructions:

- Kids drink toddy.
- Teens drink coke.
- Young adults drink beer.
- Adults drink whisky.

Make a function that receive age, and return what they drink.

### Rules:

- Children under 14 old.
- Teens under 18 old.
- Young under 21 old.
- Adults have 21 or more.

### Examples:
```
people_with_age_drink(13) == "drink toddy"
people_with_age_drink(17) == "drink coke"
people_with_age_drink(18) == "drink beer"
people_with_age_drink(20) == "drink beer"
people_with_age_drink(30) == "drink whisky"
```

## Solution:
Python
~~~
def people_with_age_drink(age):
    age_check = {
                range(0, 14) : 'drink toddy',
                range(14, 18) : 'drink coke',
                range(18, 21) : 'drink beer',
                range(21, 115) : 'drink whisky',
                }

    for key in age_check:
        if age in key:
            return age_check[key]
            break
~~~
