# 📝 Format User Data Script - Auto-Generated by Hyperbee 🚀

## Description
This script automatically formats raw user data into a structured JSON output. It ensures consistency by handling missing fields and standardizing the format.

## 🛠 Features  
✅ Formats raw user data into a clean JSON structure.  
✅ Handles missing fields gracefully (e.g., missing last names or roles).  
✅ Easy to use—just pass in raw data and get a formatted JSON output.  

## 📌 How It Works  
This script takes a list of dictionaries containing user details (e.g., `id`, `first_name`, `last_name`, `email`, `role`) and transforms them into a structured format.  

## 🛠 Installation & Usage  

### 1️⃣ Install Python (if not installed)  
Make sure you have Python installed on your system.  

### 2️⃣ Run the Script  
Save the script as `format_user_data.py` and execute it:
```sh
python format_user_data.py
```

### 3️⃣ Example Input & Output  

#### 🔹 Input (Raw Data)  
```python
sample_data = [
    {"id": 1, "first_name": "Alice", "last_name": "Johnson", "email": "alice@example.com", "role": "Engineer"},
    {"id": 2, "first_name": "Bob", "last_name": "", "email": "bob@example.com"},
]
```

#### 🔹 Output (Formatted JSON)  
```json
[
    {
        "id": 1,
        "name": "Alice Johnson",
        "email": "alice@example.com",
        "role": "Engineer"
    },
    {
        "id": 2,
        "name": "Bob",
        "email": "bob@example.com",
        "role": "N/A"
    }
]
```

## 💡 Customization  
- Modify the `format_user_data()` function to add or remove fields as needed.  
- Adjust the indentation level in `json.dumps()` for different formatting styles.  

## 📜 License  
This script is open-source and free to use. Modify it as needed!  

