This code creates a basic calculator application using Python's tkinter library for GUI development. Here’s a breakdown of its functionality:

1. GUI Setup
   It creates a main window (root) with a title "Calculator".
A text entry (ttk.Entry) displays the input and result.
The window size is 500x700 pixels (9:16 aspect ratio), and it is non-resizable.

2. Calculator Logic (handle_button_click function)
   This function processes button clicks:
"=": Evaluates the mathematical expression entered, replacing custom symbols (÷ with /, × with *).
"C": Clears the entry field.
"%": Converts the current number to a percentage (÷ 100).
"±": Negates the current number.
Any other button: Appends its value to the entry field.

3. Button Layout
   A grid of buttons is created using ttk.Button with a consistent style.
Special button behaviors:
"0" spans two columns for a larger size.
Other buttons are placed in a 4x6 grid for operations and numbers.

4. Keyboard Support
   Enter (Return) key: Triggers = (calculation).
Backspace (BackSpace) key: Triggers "C" (clear).

5. Grid Configuration
   grid_rowconfigure and grid_columnconfigure ensure the layout scales properly within the window.

6. Styling
   Uses ttk.Style() to configure button fonts and sizes.
theme_use('default') applies a default theme.

Summary
This is a fully functional, responsive, and user-friendly calculator with:
Basic arithmetic operations (+, -, ×, ÷).
Percentage and negation functions.
Keyboard shortcuts for efficiency.
Aesthetic improvements using ttk widgets.
