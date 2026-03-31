# 🚀 Logic Box Project

A simple Python console-based application that includes a **Pattern Generator** and a **Number Analyzer**.

---

## ✨ Features

- 🔹 Generate right-angled triangle pattern  
- 🔹 Analyze numbers (Odd/Even + Sum)  
- 🔹 Menu-driven interface  
- 🔹 User input handling  

---

## 📌 Project Structure

```
project.py   # Main Python file
README.md    # Project documentation
```

---

## 💻 Python Code

```python
while True:
    print("\n1. Generate Pattern")
    print("2. Analyze Numbers")
    print("3. Exit")

    choice = int(input("Enter your choice: "))

    # Pattern Generator
    if choice == 1:
        rows = int(input("Enter number of rows: "))
        for i in range(1, rows + 1):
            for j in range(i):
                print("*", end="")
            print()

    # Number Analyzer
    elif choice == 2:
        start = int(input("Enter start: "))
        end = int(input("Enter end: "))
        total = 0

        for i in range(start, end + 1):
            if i % 2 == 0:
                print(i, "Even")
            else:
                print(i, "Odd")
            total += i

        print("Sum =", total)

    # Exit
    elif choice == 3:
        print("Goodbye!")
        break

    else:
        print("Invalid choice")
```

---

## ▶️ How to Run

1. Open terminal / command prompt  
2. Run the file:
   ```bash
   python project.py
   ```
3. Follow the menu options  

---

## 🧠 Concepts Used

- for loops  
- nested loops  
- if-else conditions  
- range() function  
- break statement  

---

## 📷 Example Output

```
*
**
***
****
```

```
10 Even
11 Odd
...
Sum = 75
```

---

## 👨‍💻 Author

- Student Project
