## 🧮 Par Sheet Calculator

**Tagline**:
*Digitizing inventory communication for Fresh Truck’s mobile markets to save time, reduce errors, and improve customer service.*

---

### 📌 Project Summary

At **Fresh Truck**, I created a bespoke Google Sheets tool—the **Par Sheet Calculator**—to solve an ongoing operational inefficiency in our mobile food retail workflow. This tool modernized our inventory tracking process, reduced manual calculation errors/ frustration, and reduced the need for paper-based "par sheets."

⏱️ **Result:** Saved \~1 hour of manpower per day and redirected that time to customer service.

---

### 🛠️ Problem

Fresh Truck operates mobile markets using retrofitted school buses. Historically, staff manually filled out printed inventory sheets to estimate afternoon inventory needs based on morning leftovers.

This paper-based system was:

* Time-consuming
* Error-prone
* Frequently lost
* Disruptive to customer service during peak hours

---

### 💡 The Solution

I designed a **Google Sheets-based calculator** to digitize the process and eliminate manual steps.

🔗 [Live Sheet (View Only)](https://docs.google.com/spreadsheets/d/121EZRXI_qWhZIMNxzkgYOrmmtzyqcjMSMNIKQZWveqo/edit?usp=sharing)

#### ✅ Key Features

* Dropdown market selection triggers auto-calculation of afternoon par needs
* Live formulas using `VLOOKUP` and `IMPORTRANGE`
* Color-coded highlighting of priority quantities, does not highlight items needing .1 or -.1
* No more manual math or Slack photos of scribbled sheets

---

### 🧭 How It Works

1. **Team selects vehicle tab** (e.g. “Pina Mid-Day Inventory” or "Pam/Freedom Mid-day Inventory).
2. **User selects the afternoon market** from dropdown in cell `E1`.
3. **Morning inventory** is entered in Column B.
4. Column D **auto-calculates** how much additional product is needed.
5. Afternoon team views updated numbers instantly and prepares accordingly.

---

### ⚙️ Technical Mechanism

* `VLOOKUP` used to pull market-specific par values into Column C.
* `IMPORTRANGE` connects the locked sheet "Par by_market" to a master inventory sheet updated weekly. 
* Conditional formatting highlights priorities in Column D:

  * 🌱 1+ cases needed: dark green
  * ⚠️ Removal of excess: red text
  * 🟢 Lower needs: light green or unformatted

---

### 📈 Impact

* ✅ **1 hour saved daily**
* ✅ **No more lost sheets or illegible photos**
* ✅ **More time for customer interaction**
* ✅ **Higher accuracy in afternoon stock prep**
