# picoCTF_bloat.py_reverse_engineering_python

Add

arg432 = a[71]+a[64]+a[79]+a[79]+a[88]+a[66]+a[71]+a[64]+a[77]+a[66]+a[68]


into Function def arg133(arg432):

then you will get the flag

It looked something like this:

def arg133(arg432):
  #Flag

  arg432 = a[71]+a[64]+a[79]+a[79]+a[88]+a[66]+a[71]+a[64]+a[77]+a[66]+a[68]

  #Flag

  if arg432 == a[71]+a[64]+a[79]+a[79]+a[88]+a[66]+a[71]+a[64]+a[77]+a[66]+a[68]:

    return True #Print Happy Chance

  else:

    print(a[51]+a[71]+a[64]+a[83]+a[94]+a[79]+a[64]+a[82]+a[82]+a[86]+a[78]+\
    
a[81]+a[67]+a[94]+a[72]+a[82]+a[94]+a[72]+a[77]+a[66]+a[78]+a[81]+\

a[81]+a[68]+a[66]+a[83]) # This will print that password is incorrect
    
    sys.exit(0) #Quit the program