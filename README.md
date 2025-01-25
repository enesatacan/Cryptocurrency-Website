### 🚀 Daily JavaScript App - Day 27: Cryptocurrency Website 💰  
Part of my **Daily JavaScript Coding Challenge**, where I create a new JavaScript project every day! The aim?  
🧠 **Sharpening my skills** and ✨ **staying consistent** in coding.  

---

### 📝 Project Description  
This project is a simple and elegant website that displays **real-time cryptocurrency prices**. 💹  
It leverages the **CoinGecko API** to fetch prices for:  
- 🟠 Bitcoin (BTC)  
- 🟣 Ethereum (ETH)  
- 🐶 Dogecoin (DOGE)  

The design is **user-friendly** and follows **responsive design principles**, ensuring a seamless experience across devices.  

---

### ⚙️ Installation  

Clone or download the project files to your local machine:  
```bash
git clone https://github.com/enesatacan/Cryptocurrency-Website
```  


---

### 🛠️ Technologies Used  

- **HTML5** 🏗️: For structuring the webpage.  
- **CSS3** 🎨: For styling and layout.  
- **JavaScript** ⚡: For dynamic content and API integration.  
- **jQuery** 🔄: To simplify AJAX requests.  
- **CoinGecko API** 📡: To fetch real-time cryptocurrency prices.  

---

### 📁 File Structure  

```plaintext
├── index.html          # Main HTML file  
├── style.css           # CSS file for styling  
├── app.js              # JavaScript file for functionality  
├── images/             # Images used in the project  
│   ├── background.png  # Background image  
│   ├── bitcoin.png     # Bitcoin icon  
│   ├── ethereum.png    # Ethereum icon  
│   └── dogecoin.png    # Dogecoin icon  
```  

---

### 🌐 API Integration  

This project uses the **CoinGecko API** to fetch real-time cryptocurrency prices. The API endpoint used is:  
```
https://api.coingecko.com/api/v3/simple/price?ids=bitcoin%2Cethereum%2Cdogecoin&vs_currencies=usd
```  

#### AJAX Code Example 💻  
```javascript
const btc = document.getElementById("btc");
const eth = document.getElementById("eth");
const doge = document.getElementById("doge");

const settings = {
  async: true,
  crossDomain: true,
  url: "https://api.coingecko.com/api/v3/simple/price?ids=bitcoin%2Cethereum%2Cdogecoin&vs_currencies=usd",
  method: "GET",
  headers: {},
};

$.ajax(settings).done(function (response) {
  btc.innerHTML = response.bitcoin.usd;
  eth.innerHTML = response.ethereum.usd;
  doge.innerHTML = response.dogecoin.usd;
});
```  

---

### 📸 Screenshots  


![image](https://github.com/user-attachments/assets/32579d36-c816-49fa-b834-6839d468f14b)  

---

