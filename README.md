# JS-Conditional-Car
This script creates a dropdown menu for selecting car types and dynamically updates a paragraph element with descriptions of the selected car type using JS, providing more than two choices.

	1. Element selection: 
		○ Uses document.querySelector() to access the dropdown menu element (select) and paragraph element (p)
	2. Event Listeners:
		○ Attach a 'change' event listener to the dropdown menu using select.addEventListener("change", setCar)
		○ This will trigger the setCar function whenever the user changes the selected option.
	3. setCar function - it handles the option selection change
		○ Gets the selected value from dropdown menu using select.value
		○ Uses conditional statement (if, else if) to check selected value
		If "sedan", "suv", "hatchback", "coupe", or "truck", sets the paragraph text with specific descriptions according to the chosen type using para.textContent.
		If any other value (including the initial "--Choose One--"), clears the paragraph text (para.textContent = "").
