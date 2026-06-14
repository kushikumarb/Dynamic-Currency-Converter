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
- **API Integration:**
  - **Currency Data:** [Fawaz Ahmed's Currency API](https://github.com/fawazahmed0/currency-api) (via `cdn.jsdelivr.net`)
  - **Flag Icons:** [FlagsAPI](https://flagsapi.com/)

## 📋 How It Works

1. **Initialization:** On page load, the app populates the currency dropdowns using a global `countryList` object, default-selecting `USD` for the source and `INR` for the target.
2. **Event Listeners:** The script monitors dropdown changes to trigger flag updates and catches button clicks to calculate rates.
3. **API Integration:** - A `fetch()` request is sent to `${BASE_URL}/${fromCurr}.json`.
   - The JSON response is parsed dynamically using the key format: `data[fromCurrency][toCurrency]`.
4. **DOM Updates:** The app computes the `finalAmt` and replaces the text inside the `.msg` container.

## 🔧 Installation & Setup

To run this project locally, follow these simple steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/kushikumarb/Dynamic-Currency-Converter.git](https://github.com/kushikumarb/Dynamic-Currency-Converter.git)
2. **Navigate to the project directory**
   ```bash
   cd currency-converter
3. **Open the project**
   Simply double-click the index.html file to open it in your default browser, or use a development server extension like Live Server in VS Code.
## 📸 ScreenShots
Here are the visual outcomes of the project showing the interface and real-time updates:

| Desktop Interface | Mobile / Responsive View | Dropdown / Flag Interaction |
|---|---|---|
| ![Desktop View](results/Screenshot-1.png) | ![Mobile View](results/Screenshot-2.png) | ![Feature View](results/Screenshot-3.png) |

## 🎯 Key Learning Outcomes

- **Asynchronous JavaScript:** Mastery of `async/await` syntax and the `fetch()` API to manage live network requests.
- **Data Parsing:** Dynamically pulling multi-layered JSON keys using template literals like `data[fromCurr][toCurr]`.
- **DOM Manipulation:** Utilizing clean logic to read user inputs, create HTML elements on the fly, and modify properties instantly.
- **Error Minimization:** Sanitizing user inputs directly within the script to handle blank or negative numbers by defaulting back to `1`.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
