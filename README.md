# Prompt Password Maker

Javascript: String Generator ✨

[Click to view the deployed application](https://dieterichelizabeth.github.io/prompt-password-maker/)

This app generates random passwords after the user selects their desired criteria.
The user can pick the character length, and choose to include numbers, lowercase, uppercase, and special characters through windown prompts/confirmations.
Users are then presented with their new password on the screen.

Based on the User Story:

```
"GIVEN I need a new, secure password
WHEN I click the button to generate a password
THEN I am presented with a series of prompts for password criteria
WHEN prompted for password criteria
THEN I select which criteria to include in the password
WHEN prompted for the length of the password
THEN I choose a length of at least 8 characters and no more than 128 characters
WHEN asked for character types to include in the password
THEN I confirm whether or not to include lowercase, uppercase, numeric, and/or special characters
WHEN I answer each prompt
THEN my input should be validated and at least one character type should be selected
WHEN all prompts are answered
THEN a password is generated that matches the selected criteria
WHEN the password is generated
THEN the password is either displayed in an alert or written to the page"
```

## Screenshots

![Example password/screenshot](https://user-images.githubusercontent.com/95142863/149854056-c8a224ea-952c-4087-bf2b-14605587c957.png)

To complete this project- I created 4 arrays for available character types, and one empty array. Then created the start function with prompts for password length (validated through an if...else statement), as well as window confirms to let a user select what type of characters they want to include. Once a character type is confirmed yes/true, it is pushed into the empty array, to store the user's choices. Another if...else checks that at least one type of character was chosen to move forward. After the user's choices are stored, the array goes through a for loop (called randomizer), which grabs random values from the user's choice array, and runs through the password length selected. The .join method is then turns the result of the for loop into a string without commas. Lastly, I linked the writepassword function to the completePassword method so the string would be displayed on the page. (the writePassword function was previously provided, along with HTML and CSS files).

## Resources

- [Documentation for Data Types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
- [Documentation for Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)
- [DOM Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- [Special Characters resource](https://owasp.org/www-community/password-special-characters)
- [Array.prototype.push()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
- [Indexed collections](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections)
- [Math.random()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random#getting_a_random_integer_between_two_values_inclusive)
- [For loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)
- [Array.prototype.join()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
- [Window confirm()](https://www.w3schools.com/jsref/met_win_confirm.asp)

---

Made with ❤️  
© Liz Dieterich

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
