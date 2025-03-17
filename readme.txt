import tkinter

from tkinter import Frame,Button,Label,StringVar

root_var =tkinter.Tk()

root_var.geometry('450x450+300+100')

root_var.resizable(0,0)

root_var.title("calculator")

val = ''

data =StringVar()

root_label=Label(root_var,text='content',anchor='se',font=('verdana',20),textvariable=data)
root_label.pack(fill='both',expand=True)

def btn1_is_clicked():
    global val
    val = val +"1"
    data.set(val)
    
def btn2_is_clicked():
    global val
    val = val +"2"
    data.set(val)
    
def btn3_is_clicked():
    global val
    val = val +"3"
    data.set(val)
    
def btn4_is_clicked():
    global val
    val = val +"4"
    data.set(val)
    
def btn5_is_clicked():
    global val
    val = val +"5"
    data.set(val)
    
def btn6_is_clicked():
    global val
    val = val +"6"
    data.set(val)
    
def btn7_is_clicked():
    global val
    val = val +"7"
    data.set(val)
    
def btn8_is_clicked():
    global val
    val = val +"8"
    data.set(val)
    
def btn9_is_clicked():
    global val
    val = val +"9"
    data.set(val)
    
def btn0_is_clicked():
    global val
    val = val +"0"
    data.set(val)
    
def btnc_is_clicked():
    global val
    val = ""
    data.set(val)
    
def btnplus_is_clicked():
    global val
    val = val +"+"
    data.set(val)
    
def btnminus_is_clicked():
    global val
    val = val +"-"
    data.set(val)
    
def btnmul_is_clicked():
    global val
    val = val +"*"
    data.set(val)
    
def btndiv_is_clicked():
    global val
    val = val +"/"
    data.set(val)
    
def btnequal_is_clicked():
    global val
    val = str(eval(val))
    data.set(val)

frame1 = Frame(root_var,bg='red')

frame1.pack(fill='both',expand=True)

frame2 = Frame(root_var,bg='blue')

frame2.pack(fill='both',expand=True)

frame3 = Frame(root_var,bg='green')

frame3.pack(fill='both',expand=True)

frame4 = Frame(root_var,bg='black')

frame4.pack(fill='both',expand=True)

btn1=Button(frame1,text='1',font=('verdana',20),border=0,command=btn1_is_clicked)
btn1.pack(fill='both',expand=True,side='left')

btn2=Button(frame1,text='2',font=('verdana',20),border=0,command=btn2_is_clicked)
btn2.pack(fill='both',expand=True,side='left')

btn3=Button(frame1,text='3',font=('verdana',20),border=0,command=btn3_is_clicked)
btn3.pack(fill='both',expand=True,side='left')

btnplus=Button(frame1,text='+',font=('verdana',20),border=0,command=btnplus_is_clicked)
btnplus.pack(fill='both',expand=True,side='left')

btn4=Button(frame2,text='4',font=('verdana',20),border=0,command=btn4_is_clicked)
btn4.pack(fill='both',expand=True,side='left')

btn5=Button(frame2,text='5',font=('verdana',20),border=0,command=btn5_is_clicked)
btn5.pack(fill='both',expand=True,side='left')

btn6=Button(frame2,text='6',font=('verdana',20),border=0,command=btn6_is_clicked)
btn6.pack(fill='both',expand=True,side='left')

btnminus=Button(frame2,text='-',font=('verdana',20),border=0,command=btnminus_is_clicked)
btnminus.pack(fill='both',expand=True,side='left')

btn7=Button(frame3,text='7',font=('verdana',20),border=0,command=btn7_is_clicked)
btn7.pack(fill='both',expand=True,side='left')

btn8=Button(frame3,text='8',font=('verdana',20),border=0,command=btn8_is_clicked)
btn8.pack(fill='both',expand=True,side='left')

btn9=Button(frame3,text='9',font=('verdana',20),border=0,command=btn9_is_clicked)
btn9.pack(fill='both',expand=True,side='left')

btnmul=Button(frame3,text='*',font=('verdana',20),border=0,command=btnmul_is_clicked)
btnmul.pack(fill='both',expand=True,side='left')

btnc=Button(frame4,text='c',font=('verdana',20),border=0,command=btnc_is_clicked)
btnc.pack(fill='both',expand=True,side='left')

btn0=Button(frame4,text='0',font=('verdana',20),border=0,command=btn0_is_clicked)
btn0.pack(fill='both',expand=True,side='left')

btnequal=Button(frame4,text='=',font=('verdana',20),border=0,command=btnequal_is_clicked)
btnequal.pack(fill='both',expand=True,side='left')

btndiv=Button(frame4,text='/',font=('verdana',20),border=0,command=btndiv_is_clicked)
btndiv.pack(fill='both',expand=True,side='left')

root_var.mainloop()