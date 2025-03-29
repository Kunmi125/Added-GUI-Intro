from tkinter import * 

window = Tk()

window.geometry("500x500")
window.configure(background = "Lightgreen")





#using pack method
'''l1 = Label(window, text = "Hello World", bg = "pink", fg = "magenta", padx = 20, pady = 20)
l1.pack(padx = 20,pady = 20)

e1 = Entry(window)
e1.pack()

b1 = Button(window, text = "Click Here",bg = "Black", fg = "White")
b1.pack()

window.mainloop()'''









#Using grid method
l1 = Label(window, text = "Hello World", bg = "pink", fg = "magenta",
           font = ("comic ms sans", 15), bd = 2, # bd means border ---- specifies the width of the border
            anchor = CENTER, justify = CENTER,
            relief = RAISED,

             padx = 20, pady = 20)
l1.grid(row = 0, column = 0)

e1 = Entry(window)
e1.grid(row = 0, column = 1)

b1 = Button(window, text = "Click Here",bg = "Black",  fg = "White", relief = GROOVE, width = 10, height = 10)
b1.grid(row = 1, column = 1, columnspan = 2)

e2 = Entry(window)
e2.grid(row = 1, column = 3
        ) 
sbox = Spinbox(window, from_ = 0, to = 10 
               )
sbox.grid(row = 2, column = 0)

window.mainloop()











#Using place method
'''l1 = Label(window, text = "Hello World", bg = "pink", fg = "magenta", padx = 20, pady = 20)
l1.place(x = 50, y = 50)

e1 = Entry(window)
e1.place(x = 200, y = 200)

b1 = Button(window, text = "Click Here",bg = "Black", fg = "White")
b1.place(x = 150, y = 150)


window.mainloop()'''
