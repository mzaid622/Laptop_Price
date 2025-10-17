# 💻 Laptop Price Analysis and Prediction

## 🧠 Problem Statement
A person wants to buy a new laptop and has certain specifications in mind — such as RAM, storage type, processor, and display features.  
However, they are unsure what price range to expect for those specifications.  

This project aims to **analyze how different laptop features affect their price** and build a foundation to **predict laptop prices** based on given specifications.

---

## 🎯 Objectives
- Perform **Exploratory Data Analysis (EDA)** to understand trends in laptop pricing.  
- Clean and preprocess data to handle missing values and inconsistent formats.  
- Apply **feature engineering** to extract useful information from textual columns (e.g., CPU, GPU, ScreenResolution).  
- Identify **key factors** that influence laptop prices (RAM, storage, processor type, etc.).  
- (Optional future step) Build a **predictive model** to estimate laptop prices.

---

## 🧩 Dataset Description
The dataset contains specifications and prices of various laptops.  
**Columns include:**
- `Company` – Laptop brand  
- `Product` – Model name  
- `TypeName` – Type (Ultrabook, Gaming, Notebook, etc.)  
- `Inches` – Screen size  
- `ScreenResolution` – Display resolution and features (e.g., IPS, Touchscreen)  
- `Cpu` – Processor details  
- `Ram` – Memory size  
- `Memory` – Storage capacity and type (HDD, SSD, etc.)  
- `Gpu` – Graphics processor details  
- `OpSys` – Operating system  
- `Weight` – Weight of the laptop  
- `Price` – Target variable (price in euros)

---

## ⚙️ Steps Performed

### 1. **Data Cleaning**
- Removed unnecessary characters (e.g., “GB”, “GHz”).  
- Converted RAM and Storage to numeric values.  
- Handled missing values and inconsistent entries.  
- Extracted CPU, GPU brand, and screen-related info.

### 2. **Exploratory Data Analysis (EDA)**
- Visualized price distributions.  
- Analyzed brand-wise and type-wise average prices.  
- Explored relationships between features like RAM, CPU, Storage, and Price.  
- Checked correlations between numeric columns.

### 3. **Feature Engineering**
- Derived new features such as:
  - `Touchscreen` (binary)
  - `IPS_Panel` (binary)
  - `Resolution_Width` and `Resolution_Height`
  - `PPI` (Pixels Per Inch)
  - `CPU_Brand` and `GPU_Brand`  
- Encoded categorical variables for future modeling.

---

## 📊 Key Insights
- 💡 Laptops with **SSD storage** are significantly more expensive than HDD models.  
- 💡 **RAM size** and **CPU generation** strongly influence price.  
- 💡 **Gaming brands** (MSI, Asus, Razer) and premium models (Apple, Microsoft Surface) have higher price ranges.  
- 💡 Features like **Touchscreen**, **IPS display**, and **higher PPI** correlate with higher prices.

---

## 🧰 Technologies Used
- **Python**
- **Pandas**, **NumPy** – data manipulation  
- **Matplotlib**, **Seaborn** – data visualization  
- **Scikit-learn** (for encoding and possible modeling)

---

## 🚀 Future Work
- Implement machine learning models (Linear Regression, Random Forest, XGBoost) to predict laptop prices.  
- Deploy the model as a **web app** using Flask or Django.  
- Create an interactive **dashboard** to visualize pricing trends.

---

## 🧑‍💻 Author
**Muhammad Zaid Ashfaq**  
Data Analyst & Backend Developer  
University of Engineering and Technology (UET) Lahore  
