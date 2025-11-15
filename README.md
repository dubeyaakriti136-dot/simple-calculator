## 🧮 Simple Calculator Python Script

This is a straightforward Python script that implements a basic command-line calculator. It allows users to perform **addition, subtraction, multiplication, division, and modulo operations** on two integer inputs.

-----

### **✨ Features**

  * **Basic Arithmetic Operations:** Supports addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), and modulo (`%`).
  * **User-Friendly Interface:** Takes input for two numbers and the desired operation from the command line.
  * **Input Validation:** Handles invalid operation choices with an appropriate message.

-----

### **💻 How to Run**

1.  **Prerequisites:** Ensure you have **Python** installed on your system.

2.  **Save the Script:** Save the provided code into a file named `simple_calculator.py`.

3.  **Execute:** Open your terminal or command prompt, navigate to the directory where you saved the file, and run the script using the following command:

    ```bash
    python simple_calculator.py
    ```

4.  **Follow Prompts:** The script will prompt you for:

      * The first number (` Enter a number :-  `)
      * The second number (` Enter another number :-  `)
      * The operation choice (` enter your choice +,-,*,/,% :-  `)

-----

### **💡 Code Overview**

The script first takes two integer inputs (`a` and `b`) and an operation choice (`choice`) as a string.

```python
a =int(input("Enter a number :- "))
b =int(input("Enter another number :- "))
choice = input("enter your choice +,-,*,/,% :- ")
```

It then uses an **`if-elif-else`** structure to check the value of `choice` and perform the corresponding mathematical operation.

| Choice | Operation |
| :----: | :-------- |
| `+`    | Addition  |
| `-`    | Subtraction |
| `*`    | Multiplication |
| `/`    | Division |
| `%`    | Modulo (Remainder) |

If the entered choice does not match any of the valid operations, it prints `"invalid choice"`.

-----

### **📝 Example Usage**

```
$ python simple_calculator.py
Enter a number :- 10
Enter another number :- 3
enter your choice +,-,*,/,% :- %
1
```

(Output: $10 \pmod 3 = 1$)

-----

### **🚧 Note on Division**

  * Since the inputs are converted to integers (`int()`), the division operation (`/`) will perform **floating-point division** and the result will be a float.
  * The script **does not include error handling** for dividing by zero. Entering `0` as the second number (`b`) with the division (`/`) or modulo (`%`) choice will cause a standard Python `ZeroDivisionError`.
