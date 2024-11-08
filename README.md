# ctrl

def ctrlfinder(a):
    b = ""
    c = ""
    for i in a.split():
        if i=="Ctrl" or i=="+" or i=="C" or i=="V":
            c += " "+i
            if "Ctrl + C Ctrl + V" in c:
                b += b
                c = ""  
        else:
            b += " "+i
    print(b.lstrip())
string1 = "the egg and Ctrl + C Ctrl + V the spoon"
string2 = "WARNING! Ctrl + V Ctrl + C Ctrl + V"
string3 = "The Ctrl + C Ctrl + V Town Ctrl + C Ctrl + V"
ctrlfinder(string1)
ctrlfinder(string2)
ctrlfinder(string3)
