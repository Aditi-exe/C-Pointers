# Pointers in C

In C programming language, a pointer is a variable that holds the memory address of another variable. Pointers allow direct access to memory locations and provide a way to pass values between functions by reference.

The working of a pointer can be portrayed as follows:

![Working of a pointer](https://media.geeksforgeeks.org/wp-content/uploads/pointers-in-c.png)

In the above image, ptr is a pointer that points to the memory address of the var variable.


## Key points about pointers in C:

- Declaration: A pointer variable is declared using the '*' operator. For example, to declare a pointer to an integer variable, you would write: int *ptr;.

- Assignment: A pointer variable can be assigned the memory address of another variable using the '&' operator. For example, to assign the address of an integer variable x to a pointer variable ptr, you would write: ptr = &x;.

- Dereferencing: To access the value of the variable pointed to by a pointer, you use the '*' operator. For example, to retrieve the value of the integer variable pointed to by ptr, you would write: int y = *ptr;.

- NULL pointer: A null pointer is a pointer that does not point to any valid memory location. It is declared as NULL or 0. You should always initialize a pointer to NULL when declaring it.

- Pointer arithmetic: You can perform arithmetic operations on pointers, such as adding or subtracting an integer value to a pointer. This allows you to traverse arrays or iterate over linked lists.

- Pointers and arrays: In C, arrays are actually a type of pointer. You can use array notation to access the elements of an array, or you can use pointer arithmetic.

- Pointers and functions: Pointers are commonly used to pass arguments to functions by reference. This allows the function to modify the value of the original variable. You can also use pointers to return multiple values from a function.

- Memory allocation: C provides functions like malloc and free to dynamically allocate and deallocate memory at runtime. These functions return pointers to the allocated memory.


The syntax for using a pointer is as follows:

```
datatype *var_name; 
int *ptr;   // ptr can point to an address which holds int data
```

**NOTE**: The pointer ptr always stores integer values.  


Pointers in C can be tricky to work with and can lead to errors such as segmentation faults if not used carefully. 
