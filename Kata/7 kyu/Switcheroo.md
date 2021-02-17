# Switcheroo (Python & JavaScript solution)

## Instructions:

Given a string made up of letters a, b, and/or c, switch the position of letters a and b (change a to b and vice versa). Leave any incidence of c untouched.

##### Example:
~~~
'acb' --> 'bca'
'aabacbaa' --> 'bbabcabb'
~~~

## Solution:
Python
~~~
def switcheroo(string):  
    x = list(string)

    for i in range(len(x)):
        if(x[i] == "a"):
            x[i] = "b"
        elif(x[i] == "b"):
            x[i] = "a"

    return "".join(x)
~~~
JavaScript
~~~
function switcheroo(x){
    var a = x.replace(/a/g, "1");  
    var b = a.replace(/b/g, "a");   
    var c = b.replace(/1/g, "b");


    return c;
}
~~~
