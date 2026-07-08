# Premium Invoice Maker 🧾

A responsive, web-based invoice generator designed specifically for tours and travel agencies. It allows users to quickly add trip routes, calculate totals, preview the bill, and download a high-quality PDF invoice.

## 🚀 Features

* **Dynamic Data Entry:** Easily input passenger details, multiple routes, prices, and date.
* **Default Values:** Pre-filled fields for Vehicle Number and Driver Name (can be overridden manually).
* **Live Calculation:** Automatically calculates the grand total as you add or edit routes.
* **Inline Editing:** Click on any row in the table to directly edit passenger names, routes, or prices.
* **Instant Preview:** On-screen beautiful receipt preview before downloading.
* **High-Quality PDF Generation:** Generates a professional, print-ready PDF using `jsPDF` and `jsPDF-AutoTable`.
* **Optimized Logo Quality:** Uses HTML5 Canvas to process the logo in High-Quality PNG format, keeping the PDF size under control (Max ~5MB) without losing clarity.
* **Fully Responsive:** Works perfectly on both Desktop and Mobile devices.

## 🛠️ Technologies Used

* **HTML5:** Structure and semantics.
* **CSS3:** Custom animations, gradient backgrounds, and responsive UI.
* **JavaScript (Vanilla):** DOM manipulation, calculations, and PDF logic.
* **[jsPDF](https://github.com/parallax/jsPDF):** Client-side PDF generation (`v2.5.1`).
* **[jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable):** Table generation inside the PDF (`v3.5.31`).
* **Google Fonts:** Poppins typeface for a modern look.

## 📦 How to Use (Local Setup)

1. **Clone or Download** the repository to your local machine.
2. Ensure you have a logo file named `logo.png` in the same directory as the HTML file. *(Recommended size: 500x500px, transparent background)*
3. Double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Edge, Safari).
4. Fill in the required fields (Passenger, Route, Price).
5. Click **"Add Route"** to add it to the billing table.
6. Click **"Preview Invoice"** to see how the bill looks.
7. Click **"Download PDF"** to generate and save the High-Quality PDF to your device.

## 🎨 Customization

If you want to customize this invoice maker for a different company, you can easily modify the following in the JavaScript code:

* **Company Name:** Search for `"KRISHNA TOURS & TRAVEL"` and replace it.
* **Contact Number:** Search for `"Contact : 7457011613"` and update the phone number.
* **Theme Colors:** Modify the `primaryColor` and `secondaryColor` variables inside the `createPDFDesign` function to match your brand.
  ```javascript
  const primaryColor = [26, 42, 108]; // RGB format (Dark Blue)
  const secondaryColor = [100, 100, 100]; // RGB format (Grey)
