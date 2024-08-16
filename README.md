# jokes_python
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
