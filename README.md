# Diet_Hub_Restaurant_PythonProject
This is a simple Python program for the Diet Hub Restaurant. The program displays a menu and allows customers to add items to their order. It continuously prompts the customer for additional items until they choose to stop, and then it displays the total bill
# Diet Hub Resturant
menu = {"Salad" : 99,
        "Boiled Chicken" : 249,
        "Grilled Sandwich" : 119,
        "Sprouts" : 49,
        "Fresh Fruit Bowl" : 99
}

print("Welcome to Diet Hub Restaurant")
print("Here is our menu")
print("Salad: Rs99\nBoiled Chicken: Rs249\nGrilled Sandwich : Rs119\nSprouts : Rs49\nFresh Fruit Bowl : Rs99 ")
Total_bill = 0

while True:

    item1 = input("Enter the item you want to add: ")
    if item1 in menu:
        Total_bill += menu[item1]
        print(f"{item1} is successfully added ")
    else:
        print("Sorry this item is not currently available in our restaurant ")

    another_item = input("Do you want to add something else Yes/No: ")
    if another_item == "No":
        break
print(f"Your total bill is {Total_bill}")
print("Thanks for Visiting Our Restaurant")
