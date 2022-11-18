# object
# pip install tkinter
import tkinter as tk
import tkinter.messagebox
from tkinter.constants import SUNKEN
 
window = tk.Tk()
window.title('Calculator-GeeksForGeeks')
frame = tk.Frame(master=window, bg="skyblue", padx=10)
frame.pack()
entry = tk.Entry(master=framerelief=SUNKEN, borderwidth=3, width=30)
entry.grid(row=0, column=0, columnspan=3, ipady=2, pady=2)
 
 
def myclick(number):
    entry.insert(tk.END, number)
 
 
def equal():
    try:
        y = str(eval(entry.get()))
        entry.delete(0, tk.END)
        entry.insert(0, y)
    except:


