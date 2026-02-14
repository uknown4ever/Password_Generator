# Password Generator

A simple, clean password generator web application that creates secure random passwords based on user-defined criteria.

## Features

- **Customizable Length**: Generate passwords between 4-20 characters
- **Character Type Options**:
  - Uppercase letters (A-Z)
  - Lowercase letters (a-z)
  - Numbers (0-9)
  - Symbols (!@#$%^&*(){}[]=<>/,.)
- **One-Click Copy**: Copy generated passwords to clipboard instantly
- **Responsive Design**: Works on desktop and mobile devices

## How to Use

1. Open `index.html` in your web browser
2. Adjust the password length using the number input (default: 20)
3. Select which character types to include by checking/unchecking the boxes
4. Click "Generate Password" to create a new password
5. Click the clipboard icon to copy the password

## Files

- `index.html` - Main HTML structure
- `script.js` - Password generation logic and event handlers
- `style.css` - Styling (not included in provided code)

## How It Works

The generator uses `String.fromCharCode()` with random character codes to create truly random characters:

- **Lowercase**: ASCII codes 97-122 (a-z)
- **Uppercase**: ASCII codes 65-90 (A-Z)
- **Numbers**: ASCII codes 48-57 (0-9)
- **Symbols**: Random selection from a predefined symbol string

The algorithm ensures at least one character from each selected type is included in the password for better security.

## Browser Compatibility

Requires a modern browser with support for:
- ES6 JavaScript
- Clipboard API (`navigator.clipboard`)
- CSS3

## Installation

No installation required! Simply download the files and open `index.html` in your browser.

```bash
# Clone or download the files
# Open index.html in your browser
```

## Security Note

This generator creates passwords client-side in your browser. No passwords are sent to any server or stored anywhere. The passwords are cryptographically random based on `Math.random()`.

## License

Free to use and modify.
