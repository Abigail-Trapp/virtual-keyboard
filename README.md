# virtual-keyboard
video tutorial by dcode

The keyboard is setup as an object with three main elements, the whole body, the interractive keys area, and the individual keys themselves. 
There are two event handlers for the object's list of functions. The functions tackle what happens when the keyboard is interracted with (oninput)
 and what happens when the keyboard is closed (onclose).
The object has two properties: value in which the input is displayed in the textbox with a blank "" default and whether the keyboard is on capslock or not. 
The final elements are the keyboard's list of functions: 
    "init" which sets up the keyboard layout by creating HTML elements in JavaScript and adding to the DOM. Lines 35-38 displays the input the user provides, so whatever is typed is revealed on the page. 
    "_createKeys" which creates an empty space for the individual keys to be inserted in the keyboard body. Then the key layout is initially created as an array. 
            Icons "backspace","capslock","enter","submit", and "spacebar" are also created from the google fonts API on the HTML page and appended onto the keyboard as HTML elements.
            All the keys in the array are looped, created as buttons, and have line breaks to format them just like a keyboard.
            Classes and attributes are assigned so they can be called again.
            Switch is used for the material icon keys matching with expressions of how should they execute if they were clicked, otherwise, keys will be all lowercase unless capslock is activated.
            Keys are then appended to the created fragment, and line breaks are inserted to format the keys like a keyboard.
    "_triggerEvent" tackles the event handlers "oninput" and "onclose".
    "_toggleCapsLock" activates or inactivates capslock
    "open" opens the keyboard
    "close" hides the keyboard away from the webpage. 

I learned that "?" on lines 131 & 159 basically means "capslock will either convert text to uppercase or to lowercase". 
