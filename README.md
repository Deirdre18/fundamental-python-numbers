Good reference guide to numbers and maths in Python:

https://www.digitalocean.com/community/tutorials/how-to-do-math-in-python-3-with-operators.
https://www.mathsisfun.com/

## Types of Numbers

- What is it?

A means of categorising our data


- What does it do?

Provides a simple structure to the data that we store in memory


- How do you use it?

By declaring variables!

In Python, there are two different types of numbers that we work with on a regular basis. Up until now, we’ve mostly been looking at whole numbers. In mathematical terms, these numbers are usually integers. In computer programming, however, an integer is called an int for short. The other type of numbers that Python offers is a floating point number, or float for short. A float is a number that is followed by a decimal point. For example, a float might look like 12.74 whereas an int might be just12 or 13, depending on whether you choose to round up or not!

The reason that we need to differentiate between the two different types of numbers is so that Python can inform the computer of how much memory will need to be allocated to store that value because ints require more memory than floats. Thankfully Python will mostly work within the confines of these two types of numbers; unlike other languages such as Java or C#, which have small ints, long ints, doubles and many more! Also, in a language like Java or C#, we would have to specify the type of variable that you wish to declare.

For example, if you wanted to declare an int in C or Java you would write something like this:

int my_number = 42;

We don’t need to do this in Python. The reason for this is that Python is what we call a dynamically typed language. Therefore we don’t have to specify the type because Python will make that determination for us at runtime (while the program is running), meaning that we can focus on writing code instead of making sure we get all of our types correct! This is often referred to as duck-typing. The philosophy here is: If it quacks, treat it as duck, otherwise, handle it differently. For example, if we have a variable that contains a number that doesn’t have a decimal point, treat it as an int; otherwise, if it does have a decimal point, treat it as a float. A language that requires us to specify the type of variable that we wish to declare is called a statically typed language. Java and C# are examples of this, but we’re not going to cover those here.

# Working with different types of numbers - Park One

- What is it?

The ability to work with different types of data

- What does it do?

Gives us the ability to use different types of numbers in mathematical operations

- How do you use it?

By performing arithmetic operations on different types of data

LESSON:
So now that we’ve established that Python has different types of numbers, how do we work with them? First of all, let’s clear something up. In Python 3, whenever we use the division operator, the result will always be a float. For example:

Runnable Example


Expand

Notice that the result here is 5.0. The point accommodates the possibility that the result might not be a whole number, which we can see in this example:

Runnable Example:

15 / 3

Answer:

5.0
 

Runnable Example
 
14 / 3

Answer: 4.666666666666667

Now the result is 4.666666666666667. The number 3 doesn’t divide evenly into the number 14. The nearest number that it will divide into is 12 with a remainder of 2. Another way of wording this is that three goes into fourteen 4.666666666666667 times. If we were to use the modulo operator (%) here instead of the division operator (/), we would get a result of 2.

# Working With Different Types Of Numbers - Part Two

- What is it?

The ability to work with different types of data


- What does it do?

Gives us the ability to use different types of numbers in mathematical operations


- How do you use it?

By performing arithmetic operations on different types of data

But what if we wanted to do some division that just returns an int instead? In that case, we would use the floor division operator. Back in the Arithmetic Operators section, we saw a floor division operator that looked like this –//. It rounds the number down to the nearest whole number. For example:

Runnable Example

14 // 3

Answer: 4

As we can see, the result of 14 // 3 will return 4 (without any decimal points).

# Working With Different Types Of Numbers – Part Three
 
- What is it?

The ability to work with different types of data


- What does it do?

Gives us the ability to different types of numbers in mathematical operations


- How do you use it?

By performing arithmetic operations on different types of data

LESSON:
Now that that’s out of the way let’s look at how we can combine the two different numbers. Fortunately, Python is intelligent enough to know that floats and ints are numbers. It’s also smart enough to know that ints can’t contain decimal points. For this reason, if we add an int to a float, the result will be a float.

Runnable Example

4 + 4.0

Answer: 8


Even though 4.0 can be considered to be a whole number because it has a 0 after the decimal point, Python plays it safe and returns 8.0 anyway. Any arithmetic operation that involves an int and a float as its operands behaves the same. However, if we were to perform an arithmetic operation on two ints, then the result will be an int. Similarly, if we use two floats as our operands, then the result will be a float.

## Currency Converter
 
- What is it?

Currency Converter

- What does it do?

Converts from one currency to another

- How do you use it?

We combine mathematical techniques to create useful formulae. We would use BOMDAS if we wanted to convert currencies.

Let’s say that 1 euro is equal to 1.11 in USD. To find out how many USD one would get for 25 euro, we would just multiply 25 by 1.11.

Runnable Example
 
usd = 1.11
print(25 * usd)

Answer: 27.750000000000004

The result here is 27.750000000000004. While this may be correct, it’s not very friendly. As we know, currency is rounded to two decimal places. In order to achieve this, we need to use the round function.

Runnable Example

usd = 1.11
euro = round(25 * usd, 2)
print(euro)

Answer: 27.75

Here we’ve stored the converted and rounded value in a variable called euro. The first argument that we pass to the round function is the value that we need to be rounded, and the second argument is the number of decimal points that we want to round to. In this case, we want to round to two decimal places.

Moon Weight
 
What is it?

Moon Weight Calculator


What does it do?

Will calculate how much you weigh in the moon’s lower gravity


How do you use it?

Use multiplication to calculate weight based on known Earth to Moon gravity difference and your Earth weight.

## Moon Weight
The force of gravity on the moon is one-sixth or 16.5 times weaker than it is on earth. If we were to go to the moon, then we would weigh one-sixth of what we currently weigh here on Earth. So how would we calculate this? To calculate this, we need to multiply a value (weight) by 0.165.

Runnable Example
 
print(round(75 * 0.165, 2))

In this example, if we weighed 75 KG here on planet Earth, we would weigh 12.38 KG on the moon!

Answer: 12.38

  

  