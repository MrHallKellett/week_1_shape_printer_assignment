# Programming Project 1

## Shape Printer

---

_Write a Python program to meet these requirements:_

Your task is to create a program that will print shapes on the screen using ASCII characters.

This task can be completed as long as you have a basic understanding of loops, if/else statements, variables, data types and basic Python built-in functions and operators.

Here are some examples of shapes that could be drawn by the program:

	[default options, choice: 1]
	##
	##
	##
	##
	##
	##
	##
	##
	##
	##
	[size: 4, symbol: X, choice: 1]
	XXXX
	XXXX
	XXXX
	XXXX
	[size: 7, symbol: !, choice: 2]
	!
	!!
	!!!
	!!!!
	!!!!!
	!!!!!!
	!!!!!!!
	[size: 3, symbol: O, choice: 2]
	O
	OO
	OOO


---

### Task 1: Menu

The program should contain the following menu:

	Enter 1 for rectangle
	Enter 2 for triangle
	Enter 3 for rhombus
	Enter 4 to edit options
	Enter 5 to quit


The program should display the menu to the user and allow them to enter their choice.

The program should end if 5 is the option selected.

---

### Task 2: Display rectangle

If the user chooses option 1 from the main menu, the program should display a 10 x 10 rectangle* of "*" symbols to the user and then return back to the main menu.

_*Note that although monospace characters have a consistent width, a character's height != its width._

	Enter 1 for rectangle
	Enter 2 for triangle
	Enter 3 for rhombus
	Enter 4 to edit options
	Enter 5 to quit
	1
	**********
	**********
	**********
	**********
	**********
	**********
	**********
	**********
	**********
	**********

---

### Task 3: Display triangle

If the user chooses option 2 from the main menu, the program should display a triangle of "*" symbols to the user and then return back to the main menu. (There should be 10 symbols at the base of the triangle)

	Enter 1 for rectangle
	Enter 2 for triangle
	Enter 3 for rhombus
	Enter 4 to edit options
	Enter 5 to quit
	2
	*
	**
	***
	****
	*****
	******
	*******
	********
	*********
	**********

---

### Task 4: Edit options

If the user chooses option 4 from the main menu they should be then taken through the following options:


	Enter 1 to edit size
	Enter 2 to edit symbol
	Enter 3 to edit word

---

### Task 4a: Enter size

The user is asked to enter the size of the shape.

	Enter size: 23
	!!! Invalid size
	Enter size: 0
	!!! Invalid size
	Enter size: 8
	Size set to 8.

_This message should be repeated until the user enters a number between 2 and 10 (inclusive)._

---

### Task 4b: Enter symbol

The user is then asked to enter the symbol to draw the shape with.

	Enter symbol:
	!!! Invalid symbol
	Enter symbol: what?
	!!! Invalid symbol
	Enter symbol: ^
	Symbol set to ^.

_This input should be repeated until the user enters a SINGLE CHARACTER._

---

### Task 4c: Enter word

The user is then asked to enter a word.

	Enter word: noodlesoup
	Word set to noodlesoup.

---

### **[OR]**

	Enter word:
	No word entered.

_The user can leave this blank if they wish._

---

### Task 5: Using options

After the user has finished with the "Edit options" mode they should be taken back to the main menu.

The program should now draw shapes that are sized according to the number entered as the response to the "Enter size: " prompt.

The program should now draw shapes using the symbol provided as the response to the "Enter symbol: " prompt - _but only if no word was entered in response to the prompt at 4c... see below!_


---

### Task 6: Word shapes

When given the "Enter word: " prompt in the "Edit options" menu, the user had the opportunity to leave the word blank.

If the user leaves the word blank, the program should continue creating the shapes using the given symbol.

If the user DID enter a word, the program should now create the shapes using the word provided.

	[size: 6, symbol: *, word: "banana", choice: 1]
	banana
	banana
	banana
	banana
	banana
	banana
	[size: 4, symbol: *, word: "pineapple", choice: 1]
	pine
	pine
	pine
	pine
	[size: 8, symbol: *, word: "orange", choice: 2]
	o
	or
	ora
	oran
	orang
	orange
	orangeo
	orangeor
	[size: 10, symbol: *, word: "cat", choice: 1]
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc
	catcatcatc


---

### Task 7: Display rhombus

If the user chooses option 3 from the main menu, the program should display the following message:

	Enter slope factor: 10
	!!! Invalid slope factor.
	Enter slope factor: 4
	Slope factor set to 4.

_This message should be repeated until the user enters a valid number._

_The minimum slope factor is 1. The maximum slope factor is 2 less than the size of the shape being drawn._

Using the given symbol, size and slope factor, make the program display a rhombus.

	[size: 4, symbol: *, word: "dog", slope: 1, choice: 3]
	   dogd
	  dogd
	 dogd
	dogd
	[size: 10, symbol: ), word: "", slope: 2, choice: 3]
	                  ))))))))))
	                ))))))))))
	              ))))))))))
	            ))))))))))
	          ))))))))))
	        ))))))))))
	      ))))))))))
	    ))))))))))
	  ))))))))))
	))))))))))
	[size: 5, symbol: *, word: "apple", slope: 3, choice: 3]
	            apple
	         apple
	      apple
	   apple
	apple
	[size: 6, symbol: *, word: "egg", slope: 6, choice: 3]
	                              eggegg
	                        eggegg
	                  eggegg
	            eggegg
	      eggegg
	eggegg


