Practical List
1. Write a program to find the roots of a quadratic equation.
    CODE :
        import cmath
    
        def find_quadratic_roots(a, b, c):
            if a == 0:
                return "Coefficient 'a' cannot be zero for a quadratic equation."
            
            # Calculateing the discriminant
            d = (b**2) - (4 * a * c)
            
            # Finding the roots using cmath to handle complex numbers automatically
            root1 = (-b + cmath.sqrt(d)) / (2 * a)
            root2 = (-b - cmath.sqrt(d)) / (2 * a)
            
            return root1, root2
        
        # Input coefficients from the user
        try:
            a = float(input("Enter coefficient a: "))
            b = float(input("Enter coefficient b: "))
            c = float(input("Enter coefficient c: "))
            
            r1, r2 = find_quadratic_roots(a, b, c)
            print(f"The roots are:")
            print(f"Root 1 = {r1}")
            print(f"Root 2 = {r2}")
        
        except ValueError:
            print("Please enter valid numeric values for coefficients.")
    OUTPUT :
        Test for different types of roots :

            * **Real and Distinct Roots** ($x^2 - 5x + 6 = 0$)
                * `a = 1`
                * `b = -5`
                * `c = 6`
                * *Expected Output:* `Root 1 = (3+0j)`, `Root 2 = (2+0j)` (or float equivalents depending on execution)
    
    
            * **Real and Equal Roots** ($x^2 - 4x + 4 = 0$)
                * `a = 1`
                * `b = -4`
                * `c = 4`
                * *Expected Output:* `Root 1 = (2+0j)`, `Root 2 = (2+0j)`
    
    
            * **Complex / Imaginary Roots** ($x^2 + 4 = 0$)
                * `a = 1`
                * `b = 0`
                * `c = 4`
                * *Expected Output:* `Root 1 = 2j`, `Root 2 = -2j`

3. Write a program to accept a number ‘n’ and
a. Check if ’n’ is prime
b. Generate all prime numbers till ‘n’
c. Generate first ‘n’ prime numbers
This program may be done using functions.
4. Write a program to create a pyramid of the character ‘*’ and a reverse pyramid
5. Write a program that accepts a character and performs the following:
a. print whether the character is a letter or numeric digit or a special character.
b. if the character is a letter, print whether the letter is uppercase or lowercase
c. if the character is a numeric digit, prints its name in text (e.g., if input is 9, output is
NINE)
6. Write a program to perform the following operations on a string
a. Find the frequency of a character in a string.
b. Replace a character by another character in a string.
c. Remove the first occurrence of a character from a string.
d. Remove all occurrences of a character from a string.
7. Write a program to swap the first n characters of two strings.
8. Write a function that accepts two strings and returns the indices of all the occurrences of the
second string in the first string as a list. If the second string is not present in the first string
then it should return -1.
9. Write a program to create a list of the cubes of only the even integers appearing in the input
list (may have elements of other types also) using the following:
a. 'for' loop
b. list comprehension

10. Write a program to read a file and
a. Print the total number of characters, words and lines in the file.
b. Calculate the frequency of each character in the file. Use a variable of dictionary type
to maintain the count.
c. Print the words in reverse order.
d. Copy even lines of the file to a file named ‘File1’ and odd lines to another file named
‘File2’.
11. Write a function that prints a dictionary where the keys are numbers between 1 and 5 and the
values are cubes of the keys.
12. Consider a tuple t1=(1, 2, 5, 7, 9, 2, 4, 6, 8, 10). Write a program to perform following
operations:
a. Print half the values of the tuple in one line and the other half in the next line.
b. Print another tuple whose values are even numbers in the given tuple.
c. Concatenate a tuple t2=(11,13,15) with t1.
d. Return maximum and minimum value from this tuple

13. Define a class Employee that stores information about employees in the company. The class
should contain the following:
(i) data members- count (to keep a record of all the objects being created for this class)
and for every employee: an employee number, Name, Dept, Basic, DA and HRA.
(ii) function members:
a. __init__ method to initialize and/or update the members. Add statements to ensure
that the program is terminated if any of Basic, DA and HRA is set to a negative
value.
b. function salary, that returns salary as the sum of Basic, DA and HRA.
c. __del__ function to decrease the number of objects created for the class.
d. __str __ function to display the details of an employee along with the salary of an
employee in a proper format.

14. Write a program to define a class "2DPoint" with coordinates x and y as attributes. Create
relevant methods and print the objects. Also define a method distance to calculate the
distance between any two point objects.
15. Inherit the above class to create a "3Dpoint" with additional attribute z. Override the method
defined in "2DPoint" class , to calculate distance between two points of the "3DPoint" class.
16. Write a program to accept a name from a user. Raise and handle appropriate exception(s) if
the text entered by the user contains digits and/or special characters.


    
