from tkinter import *

oyna = Tk()
oyna.title('Kalkulyator :)')
oyna.geometry('300x300')

text = Label(text="Kalkulator :)", bg='red')
text.place(x=105, y=20, width=90, height=30)

natija = Label(text="Natija", bg='white')
natija.place(x=92, y=200, width=120, height=40)

son = Entry()
son.place(x=77, y=60, width=150, height=30)

son1 = Entry()
son1.place(x=77, y=140, width=150, height=30)



def farq():
    natija.config(text=int(son.get()) + int(son1.get()))

qoshish = Button(text='+', command=farq)
qoshish.place(x=60,y=100, width=20, height=25)

def farq1():
    natija.config(text=int(son.get()) - int(son1.get()))

ayirish = Button(text='-', command=farq1)
ayirish.place(x=100, y=100, width=20, height=25)

def farq2():
    natija.config(text=int(son.get()) * int(son1.get()))

kopayish = Button(text='x', command=farq2)
kopayish.place(x=140, y=100, width=20, height=25)

def farq3():
    natija.config(text=int(son.get()) / int(son1.get()))

bolish=Button(text=':', command=farq3)
bolish.place(x=180, y=100, width=20, height=25)

def farq4():
	natija.config(text=int(son.get()) ** int(son1.get()))

daraja=Button(text='^', command=farq4)
daraja.place(x=220, y=100, width=20, height=25)



oyna.mainloop()
