
import tkinter as tk
oyna=tk.Tk()
oyna.geometry("400x400")
oyna.title('sonlar yigindisi')
bir=tk.Label(text="Birinchi sonni kiriting")
bir.pack()
entry1=tk.Entry(oyna)
entry1.pack()
ikki=tk.Label(text="ikkinchi sonni kiriting")
ikki.pack()
entry2=tk.Entry(oyna)
entry2.pack(pady=10)
def hisobla():
    qiymat1=float(entry1.get())
    qiymat2=float(entry2.get())
    result=qiymat1+qiymat2
    natija.config(text="sum:"+str(result))
natija=tk.Label(oyna,text="Result:")
natija.pack()
button=tk.Button(oyna,text="Hisobla:", width=10,background="pink",command=hisobla)
button.pack()
insho=tk.Label(text=" Yig'indi",
foreground="blue", background="red",width=10, height=2)
oyna.configure(bg="green")
insho.pack()
oyna.mainloop()
