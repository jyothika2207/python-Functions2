# python-Functions2
#Function within the Function
def outer():
    print("Tis is a outer function.....")
    def inner():
        print("This is a inner function.....")
    inner()
outer()


======OUTPUT======
Tis is a outer function.....
This is a inner function.....
