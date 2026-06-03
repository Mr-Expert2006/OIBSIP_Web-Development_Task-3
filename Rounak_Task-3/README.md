Temperature Converter

A simple and interactive Temperature Converter web application built using HTML, CSS, and JavaScript. This application allows users to convert temperatures between Celsius (°C), Fahrenheit (°F), and Kelvin (K) instantly through a clean and user-friendly interface.

📌 Project Overview

The Temperature Converter is designed to perform accurate temperature conversions between the three most commonly used temperature scales:

Celsius (°C)
Fahrenheit (°F)
Kelvin (K)

The application takes a temperature value as input, converts it to the selected target unit, and displays the result with two decimal places.

🚀 Features
✅ Temperature Conversion

Supports conversions between:

From	To
Celsius	Fahrenheit
Celsius	Kelvin
Fahrenheit	Celsius
Fahrenheit	Kelvin
Kelvin	Celsius
Kelvin	Fahrenheit
✅ Input Validation

The application checks whether the user has entered a valid numeric value.

Example:

Please enter a valid number

If the input field is empty or contains invalid data, an error message is displayed.

✅ Instant Result Display

The converted temperature is displayed immediately after clicking the Convert button.

Example:

100° Celsius = 212.00° Fahrenheit
✅ Clean User Interface

The application features:

Dark-themed converter card
Center-aligned layout
Rounded form controls
Hover effect on buttons
Responsive and lightweight design
🛠️ Technologies Used
Frontend
HTML5
CSS3
JavaScript (Vanilla JS)

No external libraries or frameworks are required.

📂 Project Structure
Temperature-Converter/
│
├── index.html      # Main webpage structure
├── style.css       # Application styling
├── script.js       # Conversion logic
└── README.md       # Project documentation
📄 HTML Structure

The interface contains:

Title
<h2>Temperature Converter</h2>
Temperature Input Field
<input type="number" id="inputTemp">

Allows users to enter a temperature value.

Source Unit Dropdown
<select id="fromUnit">

Options:

Celsius (°C)
Fahrenheit (°F)
Kelvin (K)
Target Unit Dropdown
<select id="toUnit">

Options:

Fahrenheit (°F)
Celsius (°C)
Kelvin (K)
Convert Button
<button onclick="convertTemp()">Convert</button>

Triggers the conversion process.

Result Area
<h3 id="result"></h3>

Displays the final converted value.

🎨 CSS Styling
Page Styling
background-color: #a5b1c2;

The webpage uses a light gray-blue background.

Converter Card
background-color: #1e272e;

The converter box uses a dark theme with:

Rounded corners
Shadow effect
Internal spacing
Shadow Effect
box-shadow: 10px 20px 25px rgba(0,0,0,0.5);

Creates depth and improves visual appearance.

Heading Color
color: #4CAF50;

Green color is used for the application title.

Button Styling

Default Button:

background-color: #4CAF50;

Hover Effect:

background-color: #45a049;

Provides visual feedback when users hover over the button.

⚙️ JavaScript Logic

The conversion process is handled by the function:

function convertTemp()
Step 1: Get User Input
const inputTemp = parseFloat(...)

Reads the entered temperature value.

Step 2: Get Selected Units
const fromUnit = ...
const toUnit = ...

Retrieves the source and destination temperature units.

Step 3: Validate Input
if(isNaN(inputTemp))

Checks if the entered value is a valid number.

If invalid:

Please enter a valid number

is displayed.

Step 4: Convert Input to Celsius

The application first converts all temperatures to Celsius.

Fahrenheit → Celsius
(inputTemp - 32) * 5 / 9
Kelvin → Celsius
inputTemp - 273.15
Step 5: Convert Celsius to Target Unit
Celsius → Fahrenheit
(celsius * 9 / 5) + 32
Celsius → Kelvin
celsius + 273.15
Step 6: Display Result

The result is displayed using:

result.toFixed(2)

This ensures the output always contains two decimal places.

Example:

25° Celsius = 77.00° Fahrenheit
🔢 Conversion Formulas Used
Celsius to Fahrenheit
°F = (°C × 9/5) + 32
Fahrenheit to Celsius
°C = (°F − 32) × 5/9
Celsius to Kelvin
K = °C + 273.15
Kelvin to Celsius
°C = K − 273.15