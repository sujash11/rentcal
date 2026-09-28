# Input from user
rent = int(input("Enter your flat rent = "))
food = int(input("Enter the amount of food ordered = "))
electricity_spend = int(input("Enter the total units of electricity = "))
charges_per_unit = int(input("Enter the charges per unit = "))
persons = int(input("Enter the number of persons living in flat = "))

# Calculation
total_bill = electricity_spend * charges_per_unit
output = (rent + food + total_bill) // persons

# Final Output
print("Each person will pay = ", output)

Inputs Taken From User
	Room Rent: The total monthly amount paid for rent.
	Food Orders: Amount spent collectively on food or snacks in the month. 
	Electricity Units Spent: Number of units consumed by the household.
	Charge Per Electricity Unit: Rate per electricity unit as provided by the hostel/society. 
	Number of Persons: Total number of roommates living together.
All these values are taken one after another from the user using input prompts in Python. 
Calculation Steps
	Compute Total Electricity Bill:
Multiply the electricity units spent with the charge per unit.
For example, if 100 units are used and the charge is ₹10 per unit:
"Total Electricity Bill"=100×10="₹" 1000


	Add Up Total Expenses:
Add together:
	Room rent
	Food order amount
	Total electricity bill computed above
For example,
"Total Expenses"="₹" 5000("rent")+"₹" 2000("food")+"₹" 1000("electricity")="₹" 8000


	Divide Expenses Among Roommates:
Divide the total expenses by the number of persons living together to get each person’s share.
For 3 people,
"Share per Person"=("₹" 8000)/3≈"₹" 2666


Sample Code Structure
Here’s how the code might look, crafted entirely by hand:
python
rent = int(input("Enter your room rent: "))
food = int(input("Enter your food order amount: "))
electricity_spend = int(input("Enter electricity units spent: "))
charge_per_unit = int(input("Enter charge per unit: "))
person = int(input("How many persons are living? "))

total_electricity_bill = electricity_spend * charge_per_unit
total_expense = rent + food + total_electricity_bill
share_per_person = total_expense // person

print("Each person will pay =", share_per_person)
