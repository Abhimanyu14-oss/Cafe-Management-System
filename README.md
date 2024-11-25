☕ Cafe Management System 🛠️
Welcome to the Cafe Management System, a simple yet functional Python project designed to streamline the ordering process in a cafe or restaurant.

📜 Features
📝 Dynamic Menu: Includes items like Pizza, Pasta, Burger, Salad, and Coffee with respective prices.
🤝 Interactive Interface: Users can place an order for items from the menu and receive a summary of their total bill.
❌ Error Handling: Alerts users when an unavailable item is ordered.
📊 Real-Time Total: Keeps track of the order total dynamically.
🧩 How It Works
The program displays a welcome message along with the menu and prices.
Users input their desired items to place an order.
If the item is available, it is added to the total; otherwise, users are informed.
Users can choose to add more items to their order.
At the end, the total bill amount is displayed with a thank-you note.
📋 Menu
🍴 Item	💰 Price (Rs)
🍕 Pizza	40
🍝 Pasta	50
🍔 Burger	60
🥗 Salad	70
☕ Coffee	80
🖥️ Code Overview
python
Copy code
# Define the menu of the restaurant
menu = {
    "Pizza": 40,
    "Pasta": 50,
    "Burger": 60,
    "Salad": 70,
    "Cofee": 80
}

# Greeting
print("Welcome to Python restaurant")
print("Pizza: Rs40\nPasta: Rs50\nBurger: Rs60\nSalad: Rs70\nCofee: Rs80")

order_total = 0

# Order first item
item_1 = input("Enter the name of the item you want to order: ")
if item_1 in menu:
    order_total += menu[item_1]
    print(f"Your item {item_1} has been added to your order")
else:
    print(f"Your order item {item_1} is not available yet")

# Check if another item is needed
another_order = input("Do you want to add another item? (Yes/No): ")
if another_order == "Yes":
    item_2 = input("Enter the second item: ")
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"Item {item_2} has been added to your order")
    else:
        print(f"Order item {item_2} is not available!!")

# Display total and thank-you message
print(f"The total amount of the item(s) to pay: Rs{order_total}")
print("Thanks for visiting")

Created BY Abhimanyu Rana
email: abhimanyurana39@gmail.com
LinkedIn: www.linkedin.com/in/abhimanyurana39
