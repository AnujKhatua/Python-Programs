# Python-Program
def J():
    print("This program is made to create and edit various lists and then create a masterlist out of them ")
    c='y'
    y=1
    Masterlist = []
    while c=='y' or c=='Y':
        print("For List",y," : ")
        x=input("Enter the name of your list : \n")
        w=[]
        c1='y'
        while c1=='y' or c1=='Y':
            print("MAIN MENU","If you want to add an element type E or e",
                         "If your list is complete type C or c (NOTE: You cannot further change you list)",
                         "If you want to delete an element type D or d", sep = '\n')
            z=input()
            if z=='E' or z=='e' :
                k='y'
                while  k=='Y' or k=='y':
                    o=eval(input('Enter the Element you want to add to your list [Note: is str use quotes]'))
                    w.append(o)
                    print("The list",x," is \n",w,)
                    k=input("Do you want to add another element to your list (Y/N) \n")
            elif z=='C' or z=='c':
                c1='n'
            elif z=='d' or 'D':
                k='y'
                while k=='Y' or k=='y':
                    i=eval(input("Enter the element you want to remove from your list"))
                    if i in w :
                        w.remove(i)
                    else :
                        print("You entered an Element not in your list")
                    k=input("Do you want to delete another element from your list (Y/N) \n")
        Masterlist.append(w)
        print("Your List",x," is : \n",w,)
        print("Your Masterlist is : \n",Masterlist)
        y+=1
        c=input("Do you want to add another list to your masterlist (Y/N) \n")
    print("The Master List is : ",Masterlist,) 
