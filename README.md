## Assignment 2:
### Define details description of class and methods used in session2.py file 

#### 1. 'Something':
1. Its simply defining class which has construtor and variable initialized, 
   its getting cyclic reference which creating memory leaking in code, we need to use and manage leake instead of avoiding.

#### 2. 'SomethingNew':
1. Its New class same as Something, difference here is its just try to make cyclic reference by calling class of Something() which doing assigning as values.
   we need to manage cyclic reference to set None or to other reference while clearing memory, which increase leaks

#### 3. 'add_something':
1. This method helping to add Something() class as reference from SomethingNew which appending List object.Tries to make Cyclic reference.
2. I had fixed it by changing reference variable which making it cyclic to variable None.

#### 4. 'clear_memory':
1. Its the memory clearing method, Its simply clearing collection which was filling by add_something from Something and SomethingNew class List objects.
2. It will clear memory or remove unreference variables, which helps to break cyclic reference

#### 5. 'critical_function':
1. This test will check whether we are actually increase the memory during running the function f.
2. In this function we first filling collection first then clearing using clear_memory(). and checking runtime memory.

#### Notes: performance utility:
> Here we are suboptimally testing whether two strings are exactly same or not
> After that we are trying to see if we have a particular character in that string or not
> Currently the code is suboptimal. Write it in such a way that it takes 1/10 the current time

#### 6. 'compare_strings_old':
1. In this function we checking value of variable are same in one loop and checking character 'd' in list of variable a.
2. we using this method to check performance of running this loop using time of excecution.

#### 7. 'compare_strings_new':
1. In this function we checking variable points to same object or memory address in one loop and checking character 'd' in list of variable a.
2. we using this method to check performance of running this loop using time of excecution.

##### Difference between == and is operator in python.
is and equals(==) operators are mostly same but they are not same.
'is' operator defines if both the variables point to the same object whereas the == sign checks
if the values for the two variables are the same

#### Below the method or variable which was used as collecting or utility variables

#### 8. 'sleep':
1.We have not made any changes to it, Just commented as mentioned in file.
2. Just to pause excecution code for some time. this is just to simulate your "slow" code.

#### 9. 'char_list':
1. Its list of String object which was multiple of 200 for this case. 

#### 10 'collection':
1. Its variable of list object which was using to save list values in program.

#### 11 '__init__':
1. It construtor or intializer for class Something and SomethingNew. to initialized parameters or variables.