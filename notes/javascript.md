# Javascript

JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It works in tandom with HTML & CSS to bring about a functioning website.

### Beginner User Interaction

##### Alert

This shows a message and waits for the user to press "OK".

`alert("Hello");`

A mini-window will open with a message. This is a *modal window*, which essential means that the user can't interact with the rest of the page, press other buttons, etc, until they have dealt with the window. In this instance, it's until the user presses "OK".

##### Prompt

The function `prompt` accepts two arguments:

`result = prompt(title, [default]);`

`title`
The text to show the visitor.

`default`
An optional second parameter, the initial value for the input field.

The visitor can type something in the prompt input field and press OK. Then we get that text in the `result`. Or they can cancel the input by pressing Cancel or hitting the Esc key, then we get `null` as the `result`.

The call to `prompt` returns the text from the input field or `null` if the input was canceled.

For instance:

```
let name = prompt('What is your name?', 'Tre');
alert(`Hello ${name}!`); // Hello Tre!

```

##### Confirm

`result = confirm(question);`

The function `confirm` shows a modal window with a `question` and two buttons: OK and Cancel.

The result is `true` if OK is pressed and `false` otherwise.

For example:

```JavaScript
let isLeader = confirm("Are you a leader?");
alert(isLeader); // true if OK is pressed

```
