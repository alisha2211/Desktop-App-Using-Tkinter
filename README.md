# Desktop-App-Using-Tkinter

import tkinter as tk

def calculate():
    num1 = int(entry1.get())
    num2 = int(entry2.get())
    result = num1 + num2
    result_label.config(text=f"Result: {result}")

# Create main window
root = tk.Tk()
root.title("Simple Calculator")

# Add widgets
entry1 = tk.Entry(root)
entry1.pack()

entry2 = tk.Entry(root)
entry2.pack()

calculate_button = tk.Button(root, text="Calculate", command=calculate)
calculate_button.pack()

result_label = tk.Label(root, text="Result: ")
result_label.pack()

# Run the app
root.mainloop()

