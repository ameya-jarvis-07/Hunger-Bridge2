# 🍽 Hunger Bridge

Hunger Bridge is a web-based platform that connects **Restaurants, Citizens, NGOs, and Drivers** to fight food waste and hunger.  
The system allows restaurants and citizens to donate surplus food, NGOs to claim and distribute it, and drivers to deliver it efficiently.

---

## 🚀 Features

### Role Selection
- Centralized role selection page (`role-selection.html`).
- Roles available: **Restaurant, NGO, Citizen, Driver**.
- Database reset option (clears `localStorage`).

### Restaurant (`restaurant.html`)
- Restaurant login and dashboard.
- Add surplus food (quantity in **kg** or **units**).
- Track donation history.
- View impact summary (**meals saved** and **CO₂ reduced**) using Chart.js.
- External map link for distribution.

### NGO (`ngo.html`)
- NGO login and dashboard.
- View available food listings from restaurants/citizens.
- Claim donations for distribution.
- Track claimed food.
- View citizen suggestions (NGO location recommendations).
- Real-time alerts when new food or suggestions are added.

### Citizen (`citizen.html`)
- Citizen login as **Donator** or **Suggester**.
- **Donators**: Add surplus food with quantity (increments of 0.5 kg supported).
- **Suggesters**: Suggest new NGO locations.
- Track personal donations or suggestions.

### Driver (`driver.html`)
- Driver login and dashboard.
- View deliveries assigned when NGOs claim donations.
- Accept and mark deliveries as completed.
- Real-time updates when new deliveries are assigned.

### Python Launcher (`main.py`)
- Opens the `role-selection.html` file in the default browser.
- Allows running the platform directly via Python.

---

## 📂 Project Structure

HUNGER_BRIDGE/
│
├── role-selection.html # Entry point for role selection

├── restaurant.html # Restaurant dashboard

├── ngo.html # NGO dashboard

├── citizen.html # Citizen dashboard

├── driver.html # Driver dashboard

├── main.py # Python launcher (opens role-selection.html)


---

## 🛠 Tech Stack

- **Frontend**: HTML5, CSS3, TailwindCSS, JavaScript
- **Charts**: Chart.js
- **Storage**: Browser `localStorage`
- **Launcher**: Python (`webbrowser` module)

---

## ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/hunger-bridge.git
   cd hunger-bridge
2. Run using Python:
   ```python
   python main.py
   ```
This opens the role selection page in your default browser.

Or open role-selection.html directly in a browser.

## 📌 Notes

Data is stored in browser localStorage.
Use the Reset Database button on the Role Selection page to clear all data.

Best viewed in modern browsers (Chrome, Edge, Firefox).

Works fully offline as it does not require a backend.

## 📜 License

This project is open-source and free to use for educational and non-commercial purposes.
