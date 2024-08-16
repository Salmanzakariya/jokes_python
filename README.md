# jokes_python
Pyjokes is a Python library that generates one-liner programming jokes. It's lightweight, easy to use, and perfect for adding a bit of humor to your projects or command-line interfaces. Whether you're building a chatbot or just want a quick laugh, Pyjokes delivers tech-themed jokes with a simple function call. #Python #Pyjokes #Humor
import pyjokes
import tkinter



def enter_data():
     a= pyjokes.get_joke()
     print("* "+a)

window =tkinter.Tk()
window.title("JOKES")

frame=tkinter.Frame(window)
frame.pack()

jk=tkinter.LabelFrame(frame,text="User information")
jk.grid(row=0,column=0,padx=20,pady=10)

button=tkinter.Button(jk,text="Button",command=enter_data)
button.grid(row=3,column=3,padx=20,pady=10,)


window.mainloop()
