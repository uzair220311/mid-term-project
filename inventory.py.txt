def menu():
    print("ProductID    ProductName     Stock")
    print("1            Panadol         100")
    print("2            Surbex          100")
    print("3            Bruffin         100")
    print("4            Metformin       100")
    print("5            Naproxen        100")
    print("6            Paracetamol     100")
    print("7            Losartan        100")
    print("8            Metoprolol      100")
    order_=input("Do you want to place order: ")
    if order_=='1':
        getorder()
    if order_=='0':
        exit()    
            


def getorder():
        pid = int(input("Enter Product Id: "))
        if pid < 1 or pid > 8:
            print("Invalid id")
            exit()
        Price = int(input("Enter Price: "))
        qty = int(input("Enter Quantity: "))
        add = (Price * qty)
        print("Total bill: ", add)


print("--------------------------------------------------------")
print("---------------Welcome to Medical Inventory-------------")
print("--------------------------------------------------------")


print("1. To Display Menu \n2. To Order")
for x in range(2):
    Input = input("Enter what you want to choose: ")
    if Input == '1':
        print(menu())
    if Input == '2':
        print(getorder())
