# CSharp_calculator
Study Calculator

Methods:

1) RefreshDisplay
	Parameters: nothing
Returns: Nothing
description: Shows the "display" variable to the calculators screen.

2) PressNumber
	Parameters: number (integer)
Returns: Nothing
description: Adds the iputed character to the "display" variable + Adds the character to the "tempNumber" variable (tempNumber= concatation of tempNumber & number). Calls RefreshDisplay method.

3) Erase
	Parameters: Nothing
Returns: Nothing
description: Overrides the "display" variable with 0, erases all other temporary variables. This method will be called by the "C" button and call RefreshDisplay method.

4) Operator
	Parameters: OperationIndex (integer)
description: Called by clicking on operation button. Assigns tempNumber converted to integer to memNumber. Assigns the Operation index (given by the particular button) to memOperator.
Returns: Nothing

5) Calculate
	Parameters:	none
Returns: Nothing
description: This method will be called by pressing = button. It will give result of given mathematical operation (based on memOperator index) of memNumber and tempNumber (converted to integer). Saves the result to display variable, call RefreshDisplay method and empties the used variables.