# Helping-hand
BMS – CABA – II – Sem - IV

Important Programs – R Programming 

1. Perform maths operations on given numbers 

Ans:- 

a<- 45

b<- 50 

print(a+b) 

print(a-b)

print(a*b) 

print(a/b) 

c<-15

d<-5 

print(c^d) 

print(c%%d) 

print(c%/%d) 

----------------------------------------------------------------------------------

2. Write a function which checks whether the given number is exactly divisible by 

9.

Ans:- 

myfunction<- function(num) 

{ 

if(num%%9==0) 

{ 

print(“the given number is divisible by 9)

} 

else 

{ 

print(“the given number is not divisible by 9”) 

} 

------------------------------------------------------------------------------------------

3. Print the numbers from 1 to 50 

Ans:- 

x<- 1:50 

for(i in x) 

{ 

print(i) 

} 

-------------------------------------------------------------------------------------------

4. Print the numbers from 1 to 25 but in reverse order. 

Ans:- 

i<- 25

while(i>=1) 

{ 

print(i) 

i--

} 

---------------------------------------------------------------------------------------------

5. Write a program to print square and cube of the given number. E.g. 25 

Ans:- 

num<- 25

cat(“the square of the number is”, num^2) 

cat(“the cube of the number is”, num^3) 

---------------------------------------------------------------------------------------

6. Create a string and make use of built-in functions of string. 

Ans:- 

mystr<- “Hello, this is R”

print(“length of the string”) 

print(nchar(mystr)) 

print(grepl(“R”, mystr)) 

print(“function to concatenate the 2 strings”) 

str1<- “good”

str2<- “mornig”

paste(str1, str2) 

print(“functions to convert the string in lower and upper case accordingly”) 

print(tolower(mystr)) 

print(toupper(mystr)) 

---------------------------------------------------------------------------------------------

7. Create a list by combining vectors of employee id, names and education and 

print that list 

Ans:- 

Empid<- c(101,102,103,104,105) 

Empname<- c(“Siya”, “Raju”, “Aditya”, “Leena”, “Radha”) 

Empedu<- c(“BBA”, “BCA”, “MCA”, “MBA”, “MCM”) 

empInfo<- list(Empid, Empname,Empedu) 

print(empInfo) 

------------------------------------------------------------------------------------------

8. Create a 3X3 matrix and print it. Also print first and second row. 

Ans :- 

A<- matrix(c(1, 2, 3, 4, 5, 6, 7, 8, 9), nrow = 3, ncol = 3, byrow = TRUE) 

cat("The 3x3 matrix:\n") 

print(A) 

# Accessing first and second row 

cat("Accessing first and second row\n") 

print(A[1:2, ]) 

--------------------------------------------------------------------------------------

9. Write a program to print metrics of matrix which are dimensions, no. of rows 

and columns 

Ans:- 

# Create a 3x3 matrix 

A = matrix(c(1, 2, 3, 4, 5, 6, 7, 8, 9),nrow = 3, ncol = 3, byrow = TRUE ) 

cat("The 3x3 matrix:\n") 

print(A) 

cat("Dimension of the matrix:\n") 

print(dim(A)) 

cat("Number of rows:\n") 

print(nrow(A)) 

cat("Number of columns:\n") 

print(ncol(A)) 

cat("Number of elements:\n") 

print(length(A)) 

# OR 

print(prod(dim(A))) 

----------------------------------------------------------------------------------------

10. Create a dataframe of friend's info and print it. 

Ans:- 

# R program to create dataframe 

# creating a data frame 

Friend_data <- data.frame(friend_id = c(1:5),friend_name = c("Sachin", 

"Sourav","Dravid", "Sehwag","Dhoni"), stringsAsFactors = FALSE) 

# print the data frame 

print(friend_data) 

---------------------------------------------------------------------------------------------

11. Create the special matrices which are diagonal, identity and the matrix which 

filled by only constant value. 

Ans:- 

# R program to illustrate 

# special matrices 

# Matrix having 3 rows and 3 columns 

# filled by a single constant 5 

print(matrix(5, 3, 3)) 

# R program to illustrate 

# Diagonal matrix

# Diagonal matrix having 3 rows and 3 columns 

# filled by array of elements (5, 3, 3) 

print(diag(c(5, 3, 3), 3, 3)) 

# Identity Matrix 

# R program to illustrate 

# special matrices 

# Identity matrix having 

# 3 rows and 3 columns 

print(diag(1, 3, 3)) 

--------------------------------------------------------------------------------------------------

12. Print odd numbers from 1 to 100 using for loop. 

Ans:- 

x<-1:100 

for(i in x) 

{ 

if(i%%2!=0) 

{ 

print(i) 

} 

} 

------------------------------------------------------------------------------------------- 

13. Compare two numbers and print the bigger number. E.g. 568, 144. Make use of 

simple if-else 

Ans:- 

a<- 568 

b<- 144 

if(a>b) 

{ 

print(“a is greater than b”) 

} 

else 

{ 

print(“b is greater than a”) 

} 

------------------------------------------------------------------------------------------

14. Print even numbers from 1 to 100 using for loop. 

Ans:- 

x<-1:100 

for(i in x) 

{ 

if(i%%2==0) 

{ 

print(i) 

} 

} 

---------------------------------------------------------------------------------------

15. Create a 4X4 matrix and print it. Also print third and fourth columns. 

Ans:- 

A<- # Create a 3x3 matrix 

A = matrix(c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12),nrow = 4, ncol = 4, byrow = TRUE) 

cat("The 4x4 matrix:\n") 

print(A) 

# Accessing third and fourth column 

cat("Accessing third and fourth column\n") 

print(A[,3:4 ])

16. Draw all the plots 

Ans:- 

# drawing bar plot 

x <- c(7, 15, 23, 12, 44, 56, 32) 

# plotting vector 

barplot(x, xlab = "Age",ylab ="Count",col="white",col.axis ="darkgreen",col.lab 

="darkgreen") 

---------------------------------------------------------------------------------------------

# drawing pie chart 

# defining vector x with number of articles 

x <- c(210, 450, 250, 100, 50, 90) 

# defining labels for each value in x 

names(x) <- c("Algo", "DS", "Java", "C", "C++", "Python") 

# creating pie chart 

pie(x, labels = names(x), col = "white", 

 main = "Articles on GeeksforGeeks", radius = -1, col.main = "darkgreen") 

-------------------------------------------------------------------------------------------- 

# drawing histogram 

x <- c(21, 23, 56, 90, 20, 7, 94, 12, 57, 76, 69, 45, 34, 32, 49, 55, 57) 

# plotting

hist(x, main = "Histogram of Vector x", xlab = "Values", col.lab = "darkgreen", 

col.main = "darkgreen") 

------------------------------------------------------------------------------------------

# drawing scatter plot 

# taking input from dataset Orange already 

# present in R 

orange <- Orange[, c('age', 'circumference')] 

# plotting 

plot(x = orange$age, y = orange$circumference, xlab = "Age", ylab = 

"Circumference", main = "Age VS Circumference", col.lab = "darkgreen", 

col.main = "darkgreen", col.axis = "darkgreen") 

-------------------------------------------------------------------------------------------

# drawing boxplot 

# defining vector with ages of employees 

x <- c(42, 21, 22, 24, 25, 30, 29, 22,23, 23, 24, 28, 32, 45, 39, 40) 

# plotting 

boxplot(x, xlab = "Box Plot", ylab = "Age", col.axis = "darkgreen", col.lab = 

"darkgreen") 

--------------------------------------------------------------------------------------
