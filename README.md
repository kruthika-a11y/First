# First
Password code in python
import re
password="R@m@_f0rtu9e&$"
flag=0
while true:
  if(len(password)<8):
    flag=-1
    break
 elif not re.search("[a-z]",password):
    flag=-1
    break
 elif not re.search("[a-Z]",password):
    flag=-1
    break
 elif not re.search("[0-9]",password):
    flag=-1
    break
 elif not re.search("[_@&$]",password):
    flag=-1
    break
 elif not re.search("\s",password):
    flag=-1
    break
else:
    flag=0
    print("valid password")
    break
if flag==-1:
     print("not a valid password")
  
