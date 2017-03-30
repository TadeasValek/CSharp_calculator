# CSharp_calculator
Study Calculator

Methods:

*1) ToInteger
*	Parameters: text	(string)
*Returns: integer
*description: Converts inputed string to number for later calculation purposes/probably could be substituted by build in method 


1) RefreshDisplay
	Parameters: nothing
Returns: Nothing
description: Shows the "Display" variable to the calculators screen.

2) PressNumber
	Parameters: number (integer)
Returns: Nothing
description: Adds the iputed character to the "Display" variable + Adds the character to the "TempNumber" variable (TempNumber= concatation of TempNumber & number). Calls RefreshDisplay method.

3) Erase
	Parameters: Nothing
Returns: Nothing
description: Overrides the "display" variable with 0, erases the priorityOperation variable. This method will be called by the "C" button and call RefreshDisplay method.

4) HighPriorityOperatorButton
	Parameters: multiply (boolean)
description: Called by clicking on multiplication button (with parameter true) and divide button (with parameter false). Assigns TempNumber converted to integer by ToInteger method to memNumber, if memNumber is empty. If memNumber is not empty it assigns "memNumber" variable to "memNumber = memNumber + tempNumber (converted to integer) multiplied/divided by memNumber. Erases tempNumber.
Returns: Nothing

5) LowPriorityOperatorButton
	Parameters: add (boolean)
description: Called by clicking on the add button (with parameter true) and subtract button (with parameter false). Asigns TempNumber (converted to integer) to LowPriorityNumber1 if LowPriorityNumber1 is not empty then to LowPriorityNumber2. If 


4) SeparateNumbers
	Parameters:	Display (byte) 
Returns: array
description: This method will 
This method will store the 

5) Calculate
	Parameters:	number1		(integer)
				number2		(integer)
				operation	(string)
Returns: integer
description: This method will be called with operation input. Provide given mathematical operation with help of conditions (if multiply do number1 * number2, if divide do number1/number2) and return result as an integer.
Overrides the memNumber1 with result variable


6) Process
	Parameters: none
Returns: Nothing
description: Method calls Calculate