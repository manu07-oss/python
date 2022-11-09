# python
numerics

The types encountered so far are called primitive types. They exist in Python—a bit like atoms. These are the simplest types of variables; they are the foundation of all computer operations and programs. In the same way that atoms can be combined to make more complex molecules, you can combine primitive types to create much more complex variable types, as you will see in the next parts of this course. For now, you will explore numeric types and strings in a little more depth. Let's go!

Numeric Variables
Numeric variables can be broken down into two distinct types:

Integers, which correspond to the set of positive or negative integers (1, 2, 0, 123, -3, etc.)

Decimals, which, in addition to integers, include all decimal numbers (2.50, 5.99, -1.20, etc.)

Start with the one you are already familiar with: integers. Integers are declared like any other variable, by associating a value to a variable name.

account = 10
Here you have the value 10 associated with the variable account. 10 being an integer,  accountis automatically an integer variable (int).

For decimal numbers ,  python uses the float type. You can define it in the same way as integers, by simply adding the decimal point explicitly:

length = 1876.79
width = 870.0
As long as the associated value is a decimal number, Python will automatically consider the variable as beingfloat. This is true even if the digit after the decimal point is a 0, as is the case above with the width variable.

Mix Several Numeric Variables
It is important to keep in mind how the different numeric types can be mixed together and what the potential consequences are. If you mix different types, the most complex will be the one kept for the final result. For example, an integer value can be stored as a float, as seen above with the width variable, but the opposite is not possible if there are numbers after the decimal point! The  float  is therefore the most complex type: if you mix an   int  with a   float ,  the result will always be a   float , whatever operation is performed or whatever the result is.

a = 7.5
b = 3
c = a/b
print(c)
# this will print 2.5, which is a float
If the result of an operation between two integers is supposed to be a decimal number, Python will automatically convert it to a float. Moreover, division (even if the result is supposed to be an integer) will necessarily return a float as well:

a = 10
b = 5
c = a/b
print(c)
# it's a float
However, you can force the conversion of a variable into a well-defined type. This is called typecasting, because by doing so you are changing (casting) the type of a variable. To do this, you will need the corresponding functions:

int() : for integers

float() : for decimals
