# Convert boolean values to strings 'Yes' or 'No'. (Python solution)

## Instructions:

Complete the method that takes a boolean value and return a "Yes" string for true, or a "No" string for false.

## Solution:

Python

~~~
def bool_to_word(boolean):
    if boolean == True:
        return "Yes"
    else:
        return "No"
~~~
Or if you like one liners (Python)
~~~
def bool_to_word(boolean):
    return 'Yes' if boolean == True else 'No'
~~~

JavaScript

~~~
function boolToWord( bool ){
  if(bool == true){
    return 'Yes'
  }
  else{
    return 'No'
  }
}
~~~
