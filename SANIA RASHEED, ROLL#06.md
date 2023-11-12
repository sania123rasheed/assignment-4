### Assignment-04 (List)
- Change the notebook name with your name and Roll Number.
- Try this as your own, no chatgpt (it's for your learning)
- after completing the assignment, submit this book on google class room.

Create an empty list and print it.



```python
emp_list= list()
print(emp_list)
type(emp_list)
```

    []
    




    list



Create a list of your favorite colors and print it.



```python
colors = ["red" , "yellow" , "purple" , "green" , "voilet"]
print(colors)
type(colors)
```

    ['red', 'yellow', 'purple', 'green', 'voilet']
    




    list



Create a list that includes a mix of data types (integers, strings, floats).



```python
mixed_data = [12 , "kinza" , 61.5 , "father"]
print(mixed_data)
type(mixed_data)
```

    [12, 'kinza', 61.5, 'father']
    




    list



Access the first element of a list.



```python
new_list = [1,11,1,5,24,14,12]
print(new_list)
first = new_list[0]
print(first)
```

    [1, 11, 1, 5, 24, 14, 12]
    1
    

Access the last element of a list.


```python
len(new_list)
```




    7




```python
last = new_list[-1]
print(last)
```

    12
    

 Access the second and third elements of a list.



```python
elements = new_list[1:3]
print(elements)
```

    [11, 1]
    


Slice a list to extract the first three elements.



```python
three_elements = new_list[:3]
print(three_elements)
```

    [1, 11, 1]
    

Slice a list to extract the last three elements.



```python
last_three = new_list[-3:]
print(last_three)
```

    [24, 14, 12]
    

Slice a list to get every second element.



```python
sec_element = new_list[::2]
print(sec_element)
```

    [1, 1, 24, 12]
    

Reverse a list using slicing.


```python
reverse = new_list[::-1]
print(reverse)
```

    [12, 14, 24, 5, 1, 11, 1]
    

 Create two lists and concatenate them.



```python
list_1 = ["a","b","c","d"]
list_2 = ["e","f","g","h"]
concatenate = (list_1 + list_2)
print(concatenate)
```

    ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']
    


Repeat a list multiple times using the repetition operator


```python
list_new = ["sania"]
rep = list_new * 5
print(rep)
```

    ['sania', 'sania', 'sania', 'sania', 'sania']
    

Add a new element to the end of a list using the append() method.



```python
c_list = [1, 11,22, 33, 44]
new_element = 55
c_list.append(new_element)
print(c_list)
```

    [1, 11, 22, 33, 44, 55]
    


Extend a list with elements from another list using the extend() method.



```python
lst_1 = [9,8,7]
lst_2 = [6,5,4]
lst_1.extend(lst_2)
print(lst_1)
```

    [9, 8, 7, 6, 5, 4]
    

Insert an element at a specific index in a list using the insert() method.


```python
n_list = [10, 12, 13]
insert = 11
index = 1
n_list.insert(index, insert)
print(n_list)
```

    [10, 11, 12, 13]
    

 Remove the last element from a list using the pop() method.




```python
List = [9,8,7,6]
last_elem = List.pop()
print("Removed Element:", last_elem)
print("updated List:", List)
```

    Removed Element: 6
    updated List: [9, 8, 7]
    

Remove a specific element from a list using the remove() method.



```python
print(List)
remove_elem = 8
rem = List.remove(remove_elem)
print("updated List:", List)
```

    [9, 8, 7]
    updated List: [9, 7]
    

Clear all elements from a list.



```python
create_list = [66,77,88,99]
print(create_list)
clear = create_list.clear()
print("Updated List:", create_list)
```

    [66, 77, 88, 99]
    Updated List: []
    

Delete an element at a specific index using the del statement.


```python
LIST = [22,33,44,55]
index_to_del = 3
del LIST[3]
print("Updated List:", LIST)
```

    Updated List: [22, 33, 44]
    

Convert a string to a list of characters and vice-versa.


```python
string_value = "SANIA RASHEED"
list_character = [char for char in string_value]
print(list_character)
```

    ['S', 'A', 'N', 'I', 'A', ' ', 'R', 'A', 'S', 'H', 'E', 'E', 'D']
    


```python

Sort a list in descending order using the sort() method.

```


```python
a_list = [16, 13, 12, 17, 98]
a_list.sort(reverse = True)
print("Sorted List (Descending):", a_list)
print(a_list)
```

    Sorted List (Descending): [98, 17, 16, 13, 12]
    [98, 17, 16, 13, 12]
    

Reverse the order of a list using the reverse() method.



```python
my_lst = [43,67,96,24,90]
rev = my_lst.reverse()
print(my_lst)
```

    [90, 24, 96, 67, 43]
    

Check if an element is present in a list using the in operator.


## CONDITION 1:- 


```python
b_list = [10,29,38,47,56]
elem_to_check = 47
if elem_to_check in b_list:
    print(f"{elem_to_check} is present in the list.")
else:
    print(f"{elem_to_check} is not in the list.")
```

    47 is present in the list.
    

## CONDITION 2:-


```python
b_list = [10,29,38,47,56]
elem_to_check = 50
if elem_to_check in b_list:
    print(f"{elem_to_check} is present in the list.")
else:
    print(f"{elem_to_check} is not in the list.")
```

    50 is not in the list.
    

Compare two lists to see if they are equal in both value and identity.


## CONDITION 1:-


```python
listed1 = [1, 2, 3, 4, 5]
listed2 = [1, 2, 3, 4, 5]
if listed1 == listed2:
    print("The lists are equal in value.")
```

    The lists are equal in value.
    

## CONDITION 2:- 


```python
listed3 = [1, 2, 3]
listed4 = [1, 2, 3]
listed3 = listed4
if listed3 is listed4:
    print("The lists are identical in memory.")
else:
    print("The lists are not identical.")
```

    The lists are identical in memory.
    

Create a shallow copy of a list and modify one of the lists to observe the effects on the other.



```python
original = [12, 11, 10, 9, 8]
shallow_copy = original[:]
original[0] = 9
print("Original:", original)
print("Shallow Copy:", shallow_copy)
```

    Original: [9, 11, 10, 9, 8]
    Shallow Copy: [12, 11, 10, 9, 8]
    

Create a deep copy of a nested list and modify one of the lists to observe the effects on the other.


```python
import copy
nested_list = [[12, 13], [14, 15]]
deep_copy = copy.deepcopy(nested_list)
nested_list[0][0] = 16
print("Nested List:", nested_list)
print("Deep Copy:", deep_copy)
```

    Nested List: [[16, 13], [14, 15]]
    Deep Copy: [[12, 13], [14, 15]]
    

Pickle and Unpickle a list and display its content.


```python
import pickle
k_list = [0, 12, 1, 11, 24]
with open('k_list.pickle', 'wb') as file:
    pickle.dump(k_list, file)
with open('k_list.pickle', 'rb') as file:
    unpickled_list = pickle.load(file)
print("Unpickled List:", unpickled_list)
```

    Unpickled List: [0, 12, 1, 11, 24]
    


```python

```
