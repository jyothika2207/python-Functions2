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




# python- addition,subtraction,multiplication in Functions2
def cal(a,b):
    def add():
        return a+b
    def sub():
        return a-b
    def mul():
        return a*b
    print("Addition ",add())
    print("Subtraction",sub())
    print("Multiplication",mul())
a=int(input("enter a number"))
b=int(input("enter b number"))
cal(a,b)



======OUTPUT======
enter a number 45
enter b number -19
Addition  26
Subtraction 64
Multiplication -855





def greet(text):
    def inner (name):
        return f" {text},{name}!!!!!"
    return inner
hi=greet('Hello')
print(hi('Jyothika'))



==========OUTPUT========
Hello,Jyothika!!!!!







number =int(input("enter the number:"))
if is_prime(number):
    print(f"{number} is a prime number.")
else:
    print(f"{number} is not a prime number.")

    ========OUTPUT=======
    enter the number: 3
    3 is a prime number.




    def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        print(a, end=' ')
        a, b = b, a + b

n = int(input("Enter the number of terms: "))
fibonacci(n)


=======OUTPUT=============
Enter the number of terms:  7
0 1 1 2 3 5 8 




def titled(title):
    def greet(name):
        return f"Hello, {title}{name}"
    return greet
mr_greet=titled("Mr.")
dr_greet=titled("Dr.")
print(mr_greet("Jyothika"))
print(dr_greet("joshika"))

=======OUTPUT=========
Hello, Mr.Jyothika
Hello, Dr.joshika




