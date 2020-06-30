### Programacion funcional en Python

Programacion funcional en Python, al estilo del pensamiento matematico: todo en base de fuciones a las que se proporciona parametros y devuelve resultados al aplicar la funcion. En el codigo de la funcion, el resultado depende unicamente de los parametros pasados.

**Lambda**

lambda operator or lambda function is used for creating small, one-time and anonymous function objects in Python.

example syntax

```Python
add = lambda x, y : x + y  
print add(2, 3)
type(add)

#Output 
5
function
```
**map**

map executes the function_object for each element in the sequence of iterables in a list or a dictionary and returns a list of the elements modified by the function object.
```Python
map(function_object, iterable1, iterable2,...)
```
example syntax
```Python
multiply2 = lambda x:x * 2
print multiplied = map(multiply2, [1, 2, 3, 4])#Output 
[2, 4, 6, 8]
```
this could even be written in one line as:
```Python
map(lambda x : x*2, [1, 2, 3, 4]) 
#Output [2, 4, 6, 8]
```
multiple lists also could be iterated:
```Python
list_a = [1, 2, 3]
list_b = [10, 20, 30]  
map(lambda x, y: x + y, list_a, list_b)# Output
[11, 22, 33]
```
see another example to run functions is sequence:
```Python
def func1():
    pass

def func2():
    pass

def func3():
    pass

func_exec = lambda f: f()
map(func_exec, [func1, func2, func3])
```
