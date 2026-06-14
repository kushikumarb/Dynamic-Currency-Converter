# Dynamic Currency Converter

A lightweight, responsive web application that provides real-time currency conversion rates. This project fetches live exchange data from a public financial API and allows users to seamlessly convert amounts between different global currencies.

## 🚀 Features

- **Live Exchange Rates:** Fetches up-to-date currency data using the native JavaScript Fetch API.
- **Dynamic UI:** Automatically updates country flags when a new currency is selected from the dropdown.
- **Instant Conversion:** Calculates and displays the converted amount accurately with a single click.
- **Responsive Design:** Optimized for a seamless experience across mobile, tablet, and desktop screens.
- **Robust Error Handling:** Includes fallback mechanisms to handle network failures or API limits gracefully.

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3 (Flexbox/Grid)
- **Scripting:** JavaScript (ES6+)
- **API Integration:** Fetch API / Async-Await

## 📋 How It Works

1. The user enters the desired amount to convert.
2. The user selects the **From** (source) and **To** (target) currencies from the dropdown menus.
3. The JavaScript script listens for the submission event, triggers an asynchronous `fetch()` request to the exchange rate API, and parses the JSON response.
4. The DOM is dynamically updated with the converted amount and the corresponding country flags.

## 🔧 Installation & Setup

To run this project locally, follow these simple steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/currency-converter.git](https://github.com/your-username/currency-converter.git)
   ```
2. **Navigate to the project directory**
   ```bash
   cd currency-converter
   ```
3. **Open the project**
   Simply double-click the index.html file to open it in your default browser, or use a development server extension like Live Server in VS Code.
## 📸 ScreenShots
