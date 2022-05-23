# Joash-Miguel-Dolor_FinalExam- 

from tkinter import *


def number():
    if num1 < num2 and num1 < num3:
        print("{} is smallest".format(num1))
    elif num2 < num3:
        print("{} is smallest".format(num2))
    else:
        print("{} is smallest".format(num3))


class Number:
    def __init__(self, win):
        self.num1 = Label(win, text="Enter 1st Number:")
        self.num1.place(x=25, y=25)
        self.enum1 = Entry(bd=3)
        self.enum1.place(x=140, y=25)
        self.num2 = Label(win, text="Enter 2nd Number:")
        self.num2.place(x=25, y=60)
        self.enum2 = Entry(bd=3)
        self.enum2.place(x=140, y=60)
        self.num3 = Label(win, text="Enter 3rd Number")
        self.num3.place(x=25, y=95)
        self.enum3 = Entry(bd=3)
        self.enum3.place(x=140, y=95)
        self.snum = Button(win, text="The smallest number among the three is ", command=self.number)
        self.snum.place(x=25, y=140)
        self.snum = Entry(bd=3)
        self.snum.place(x=140, y=140)


window = Tk()
gui = Number(window)
window.title("Final Exam")
window.geometry("300x200+10+10")
window.mainloop()
