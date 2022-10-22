# Assignment-

Problem statement 1: Write python code
A restaurant keeps a log of (eater_id, foodmenu_id) for all the diners. The eater_id
is a unique number for every diner and foodmenu_id is unique for every food item
served on the menu. Write a program that reads this log file and returns the top 3
menu items consumed. If you find an eater_id with the same foodmenu_id more
than once then show an error.

Approach - I have made the dictionary with eater_id as key and foodmenu_id as value.
And then I have traversed through all the keys to append the food items in the list.
Then found the count of each food item, argsort it to find the top 3 counts.
And returned the top 3 food items.

{ eater_id_1:foodmenu_id_1,
  eater_id_2:foodmenu_id_2 }
  
Added the test cases to test codem and it is going well.


Problem 2: Debug the python code and fix it.
The task of the following code is to build a tree and print it. However, during
printing the code goes in an infinite loop.
a) Identify why it goes in infinite loop
b) Provide a fix

A)The reason of going to infinite loop is- Whenever we are initialising the node class object, we are not taking the children attribute.
The children are making for the entire class , instead we have to make it for the node specific.

B)Added the code of children=[],self.children=children , so that the children is being made for the node specific.
![tree](https://user-images.githubusercontent.com/84618439/197336071-8ea88b53-e74f-434d-94e2-5902538289c8.png)
