# 🛒 Sell Page – Farmily Marketplace

## 📌 Overview

The **Sell Page** is the heart of Farmily’s digital mandi. It allows verified farmers to list their crops directly for buyers — **without middlemen exploitation**. Unlike other platforms, Farmily ensures **authenticity and fair pricing** by enforcing mandi-based price bands.

This creates a **transparent, farmer-first marketplace** where buyers trust what they see, and farmers get a fair share of income.

---
 
## ⚙️ Key Features

### ✅ 1. Verified Farmer Login

* Farmers must log in using **Kisan ID/Aadhaar-based verification**.
* Prevents fake sellers and ensures **only genuine farmers can list produce**.

### ✅ 2. Produce Listing Form

* Farmers enter:

  * Crop Name
  * Quantity (kg/ton)
  * Location (village, district)
  * Price (must be within mandi range)
  * Optional: Product photo

### ✅ 3. Price-Band Enforcement

* Farmily fetches **min–max mandi price** for that crop using **data.gov.in API**.
* Farmer’s entered price must be **within this band**.
* Prevents **fake/unrealistic listings** (e.g., ₹2 for 100kg cashews).
* Works like the **FIFA player card market system**, ensuring trust.

### ✅ 4. Real-Time Validation

* If price is out of range → system blocks submission.
* Farmer gets a message: *“Please set your price between ₹X and ₹Y (current mandi price band).”*

### ✅ 5. Listing Display

* Once approved, the product appears in the **Farmily Marketplace**.
* Buyers see:

  * Crop Name
  * Price (farmer-set, within range)
  * Location
  * Quantity
  * Farmer Verification Badge ✅

### ✅ 6. Buyer Interaction

* Buyers can **browse listings**, filter by crop, location, or price.
* Buyers place an **order request**, which the farmer accepts/rejects.
* Future scope: Integrated payment gateway + blockchain-backed receipts.

---

## 🔄 Workflow (Step by Step)

1. **Farmer Login** → Verified by Kisan ID/Aadhaar.
2. **Farmer Adds Produce** → Enters details into Sell Page form.
3. **System Fetches Mandi Price Band** → From govt API.
4. **Validation** → Price auto-checked against mandi min–max.
5. **Listing Approved** → Product shown in marketplace.
6. **Buyer Browses & Orders** → Verified, trusted transaction begins.

---

## 🏗️ Tech Stack

* **Frontend:** HTML, CSS (Tailwind), JavaScript
* **Backend (Prototype):** Node.js + Express
* **Database:** MongoDB (stores farmer listings & user profiles)
* **APIs:**

  * **data.gov.in** → mandi min–max prices
  * **OpenWeather API** → shown alongside crop listing for planning (contextual info)
* **Future:** Blockchain records for transaction history

---

## 🔐 Why This Matters

* **Trust Building:** Buyers only see **realistic, validated prices**.
* **Fair Income:** Farmers cannot be undercut below mandi minimums.
* **Transparency:** Every listing comes from a **verified farmer**, no fake accounts.
* **Scalable Model:** Works across different crops, regions, and seasons.

---

## 📊 Example Scenario

* A farmer wants to sell **100kg of Tomatoes**.
* Current mandi price band = **₹8 – ₹12/kg**.
* Farmer enters: **₹10/kg** → Accepted ✅
* If farmer enters: **₹3/kg** → Rejected ❌ (prompt shows “Please set between ₹8–₹12”).
* Listing goes live → Buyer sees verified farmer profile + ₹10/kg price.
* Buyer places order → transaction recorded.

---

## 📌 Future Enhancements for Sell Page

* **Photo Upload:** Farmers upload crop photos for buyer confidence.
* **AI Price Advisor:** Suggests best price within mandi band.
* **Blockchain Integration:** Immutable record of every listing.
* **Smart Contracts:** Automated payment release on delivery confirmation.
