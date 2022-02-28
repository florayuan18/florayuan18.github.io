---
layout: page
title: Flora Reflection
subtitle: Flora
---

## Individual Feature Reflection
- I think I was somewhat successful in making my feature.  The overall goal of the feature was to create a login/register system that would allow users to see their respective games + ratings for those games.
  ![loginTest](/assets/img/loginTest.png)
- I intially wanted to use the features in Spring along with a MySQL database, but I quickly found out that it would be a little too complex at my current level, so I switched to a different way of going about the issue.
- I ended up using JSON data, creating five users that were stored in the login html page.  Basically, the user would have to input their username and password.  If both the username and password matched the JSON information, then the user would be taken to a separate page that displayed the games and ratings in the original JSON information.
  ![jsonData](/assets/img/jsonData.png)
- I used for loops and if/else statements to check if the username/password matches with the JSON data, as well as display alerts if the username or password does not exist.
  ![noUsername](/assets/img/noUsername.png)
  ![noPassword](/assets/img/noPassword.png)
- I converted the JSON data dynamically to an HTML table using Javascript, which ended up working well.
  ![personTest](/assets/img/personTest.png)
  ![personTable](/assets/img/personTable.png)
- I think what I lacked in the individual feature was both design and functionality.  When I tried to reformat the login page in a fancier way, it wouldn't jump to the html table.  Additionally, I had the information stored within the html instead of a separate Users.json file which would have made the code easier to read.
- If I were to add on to this feature, I would want to add the register aspect of it, as I wasn't able to figure out how to allow the users to create their own accounts with the method I employed.
- As a whole, working on this feature allowed me to bolster my understanding of how programs store data.  Additionally, I enjoyed the trial and error process of figuring out how to implement this feature, as it forced me to ensure my entire plan would work before putting effort into something that would have yielded no results.

## FRQ 1 - Unit 2 Light Sequence
- Unit 2 focused on using objects, so I learned how to create these objects and implement them to use math functions.
- This was the first time I really worked with String [] args & the scanner, so it was interesting trying to figure that out.

## FRQ 2 - Unit 3 Dinner
- Unit 3 focused on boolean expressions and if statements
- I learned how to use these expressions/statements to guides a program to make decisions based on specified criteria.
- I feel like this program probably isn't very helpful in real life because of how simple it is, since it just returns the food selection based on the number the user puts in.  Maybe if the values were stored in a database it would probably be better.

## FRQ 3 - Unit 4 Longest Streak
- Unit 4 focused on iteration
- By doing this FRQ, I became more familiar with the format of a for loops and working with nested iteration
- Parts for the header: initialization (int i = 1), boolean expression (i < input.length), and increment/decrement (i++ or i--)

## FRQ 4 - Unit 4 Coin Game
- Unit 4 focused on iteration 
- By doing this FRQ, I learned how become more familiar with creating the while loops.
- I incorporated if statements in order to guide the program 

## FRQ 5 - Unit 5 Invitation
- Unit 5 focused on writing classes
- I learned how to set up classes as well as use concatenation to display for the frontend.

## FRQ 6 - Unit 5 Password Generator
- Unit 5 focused on writing classes
- I learned how to set up the different components of a class, namely using the "this keyword" and using for loops to generate the password (i++) 

## FRQ 7 - Unit 6 Payroll
- Unit 6 focused on arrays
- I learned how to set up an array with the given College Board values
- I learned how to traverse the array using a for loops
- As the for loop moves on, it goes through each place on the array, starting with 0.  The array goes through.  If the condition in the if statement is satisfied, the integer is set to the value in the array.

## FRQ 8 - Unit 7 Username
- Unit 7 focused on arraylists and sorting
- I learned how to traverse the array list using for loops, as well as more about how to use boolean values within loops.

## FRQ 9 - Unit 8 Experimental Farm
- Unit 8 focused on the difference between 1D and 2D arrays, as well as traversing 2D arrays.
- I learned how to implement and traverse 2D arrays, as well as how to use min and max functions.

## FRQ 10 - Unit 9 Books
- Unit 9 focused on superclasses and subclasses, as well as using the super keyword.
- I learned how to use "extends" to extend PictureBook from Book.  I also learned how to use the super keyword to refer to the objects from the class I was extending.

## FRQ 11 - Unit 9 Animals
- Unit 9 also focused on polymorphism and overriding.
- I learned how to implement the grandchild class (with elephants).

## FRQ 12 - Unit 10 Number System
- Unit 10 focused on recursion, specifically with searching and sorting.
- I learned how to compare numbers, as well as search for the greatest common factor.