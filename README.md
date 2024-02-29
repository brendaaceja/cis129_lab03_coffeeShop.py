# Get input from customer
print('What are you purchasing today?')
nameOfFirstItem = input("Enter the name of the first item: ")
nameOfSecondItem = input("Enter the name of the second item: ")
numberOfCoffeesPurchased = int(input("Enter the number of coffees purchased: "))
numberOfMuffinsPurchased = int(input("Enter the number of muffins purchased: "))
priceOfFirstItem = float(input("Enter the price of the first item: "))
priceOfSecondItem = float(input("Enter the price of the second item: "))
priceOfTax = float(input("Enter the tax amount: "))

#After recieving the appropritate responses, we will move onto getting the total cost
# Calculate total cost

totalCost = (numberOfCoffeesPurchased * priceOfFirstItem) + (numberOfMuffinsPurchased * priceOfSecondItem)
totalCostWithTax = totalCost + priceOfTax

# Display the receipt
print('**************************')
print('My Coffee and Muffin Shop')
print('Number of Coffees Bought:', numberOfCoffeesPurchased)
print('Number of Muffins Bought:', numberOfMuffinsPurchased)
print('**************************')
print('**************************')
print('My Coffee and Muffin Shop Receipt')
print(numberOfCoffeesPurchased, 'Coffee at', priceOfFirstItem, 'each:', numberOfCoffeesPurchased * priceOfFirstItem)
print(numberOfMuffinsPurchased, 'Muffins at', priceOfSecondItem, 'each:', numberOfMuffinsPurchased * priceOfSecondItem)
print('6% Tax:', priceOfTax)
print('-----------------')
print('Total Cost:   ', totalCostWithTax)
print ('*************************')
