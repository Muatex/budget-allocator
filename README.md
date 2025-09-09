# Budget Allocator
- [Features](#-features)  
- [How to Use](#-how-to-use)  
- [Notes](#-notes)  
- [Usage](#-usage)  

![Budget Allocator](https://lab.muatex.com/tools/budget-allocator/og-image.png)

A lightweight budgeting tool that runs in your browser. Nothing leaves your machine with zero servers, accounts, or tracking.  

👉 [See a Live Demo](https://lab.muatex.com/tools/budget-allocator-demo/)

---

## ✨ Features

### 📌 Fixed amounts  
Set recurring costs that come off the top every time. Examples: phone bill, groceries, utilities.  

### 📊 Percent allocations  
Split what’s left into categories by percentage. Works with decimals (`0.25`) or whole numbers (`25`). Good for savings, charity, pocket money, or anything else that shifts with your income.  

### 🔢 Rounding  
Choose the step for rounding (e.g. 5, 10). Keeps numbers clean, automatically balances small differences.  

### 💱 Currency  
Pick any symbol: `£`, `$`, `€`, or another. All calculations adapt.  

### 📝 Notes  
Short reminders for where each amount goes: “ATM”, “Bank”, “Send to Mum”. They sit under each row, so you don’t forget the destination.  

### 📋 Clipboard copy  
Click any row and the number is copied. Handy for transferring amounts into banking apps or notes without retyping.  

### 🎨 Theme customisation  
Tweak the look in `index.html` under `:root`:  
- Colours (background, text, accent)  
- Fonts (Inter, Roboto Mono, or your own)  
- Border radius and spacing  
- Highlight behaviour  

### 💻 Local & static  
Runs from a single HTML + JSON setup.  
Because it uses `config.json`, it needs to be opened through a simple server, not just by double-clicking the file.  

**Easy options:**  
- **Quick local run:**  
  - If you have Python, open the folder and type:  
    `python -m http.server`  
    Then go to [http://localhost:8000](http://localhost:8000).  
- **Host online for free:**  
  - Drop the folder onto services like **Vercel**, **Netlify**, **Firebase Hosting**, or **GitHub Pages**.  
  - They’ll give you a link to use it anywhere.  

No complicated setup is required — it’s just about serving the files instead of opening them directly.  

### 📅 Fits monthly rhythm  
Made to be used once a month when your paycheck comes in. Especially useful if your priorities or income change — just edit `config.json` and refresh.  

---

## 🛠 How to Use
1. Run the project locally or host it (see above).  
2. Open `index.html` in your browser.  
3. Enter your income.  
4. Fixed amounts are deducted first.  
5. The remainder is split by your percentages.  
6. Click rows to copy amounts where you need them.  
7. To customise:  
   - Open **`config.json`** in any text editor.  
   - Edit the values:  
     - **currency** → symbol shown (e.g. £, $, €).  
     - **roundingIncrement** → smallest step to round allocations.  
     - **fixed** → exact amounts always deducted (with short notes for where to send them).  
     - **percent** → split of what’s left, defined as percentages (each with a note for where to send).  
   - Save the file and refresh the page — your changes apply instantly.  

---

## 📎 Notes
- Percentages should add up to 100. If not, you’ll see a warning.  
- If fixed costs exceed your input, the remainder is zero.  
- Each instance is yours alone: edit config and theme to shape it how you want.  

---

## Usage

This project is shared for **personal use**.  
The idea is that everyone runs their own instance, customised to their own budget and design. It isn’t meant as a product to sell or distribute, especially not in bulk.  

Feel free to download it, edit it, and run it for yourself.  
Please **do not** repackage, resell, or publish it as your own — the code and design remain the property of **Muatex Media**.  

---

© Muatex Media. All rights reserved.  
