# project1-demo on Python
This is my first git repository.
<br>
Author-Sayani Maity
#Define the menu of resturant
menu = {
    'Pizza':40,
    'Pasta':50,
    'Burger':60,
    'Salad':70,
    'Coffe':80, 
}

#Greet
print("Welcome to PYTHON Resturent")
print("Pizza: Rs40\nPasta:Rs50\nBurger:RS60\nSalad:Rs70\nCoffe:Rs80")

order_total = 0
#40 + 70 = 110

item_1 = input("Enter the name of item you want to order = ")
if item_1 in menu:
    order_total += menu[item_1] #0 + 50
    print(f"Your item{item_1} has been added to your order")
else:
    print(f"Ordered item {item_1} is not available yet!")
       
another_order = input("Do you want to another item? (Yes/No)")
if another_order =="Yes":
    item_2 = input("Enter the name of second item =")
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"Item {item_2} has been added to order")
    else:
        print(f"Ordered item{item_2} is not available!")
        
print(f"The total amount of item to pay is {order_total}")
