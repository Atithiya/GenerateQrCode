# GenerateQrCode

# QR Code Generator

This is a simple HTML web page for generating QR codes based on user input. Users can enter text or a URL, and when they click the "Generate QR Code" button, a QR code image is displayed on the page. This README provides an overview of the code and how it works.

## Code Explanation

### HTML Structure

- `<!DOCTYPE html>`: The document type declaration for HTML5.
- `<html lang="en>`: The opening tag for the HTML document with the language attribute set to English.
- `<head>`: Contains metadata and links to external resources.
- `<body>`: The main content of the web page.

### Page Elements

- `<input>`: This is where users enter the text or URL for generating the QR code. It has an `id` of "qrText".
- `<img>`: An empty `<img>` element with the `id` of "qrImage" where the generated QR code will be displayed.
- `<button>`: A button with an `onclick` attribute that calls the `generateQR()` function when clicked.

### JavaScript

- The JavaScript code is embedded in the `<script>` tag within the HTML document.
- The code selects the HTML elements using their `id` attributes and assigns them to variables for easy access.
- The `generateQR()` function is called when the "Generate QR Code" button is clicked.
- It checks if the input field (`qrText`) has a value. If it does, it generates a QR code using the `qrserver` API and displays it in the `<img>` element.
- If the input field is empty, it adds a CSS class to the input field to highlight the error and removes it after 1 second.

## Potential Issues

- The code uses the `qrserver` API to generate QR codes. You might run into CORS issues, so consider hosting the QR code generation code on your server or find an API that allows cross-origin requests.
  (https://goqr.me/api/)
