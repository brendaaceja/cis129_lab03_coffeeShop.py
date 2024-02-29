# Get input from customer
firstItem = "coffee"
secondItem = "muffin"
thirdItem = "tea"
fourthItem = "cookie"
coffeesPurchased = 1
muffinsPurchased = 2
teaPurchased = 2
cookiesPurchased = 1
priceCoffee = 5
priceMuffins = 4
priceTea = 6
priceCookies = 3
priceTax = 0.78

print('What are you purchasing today?')
nameOfFirstItem = input("Enter the name of the first item (default: coffee): ") or firstItem
nameOfSecondItem = input("Enter the name of the second item (default: muffin): ") or secondItem
nameOfThirdItem = input("Enter the name of the third item (default: tea): ") or thirdItem
nameOfFourthItem = input("Enter the name of the fourth item (default: cookies): ") or fourthItem
numberOfCoffeesPurchased = int(input("Enter the number of coffees purchased (default: 1): ") or coffeesPurchased)
numberOfMuffinsPurchased = int(input("Enter the number of muffins purchased (default: 2): ") or muffinsPurchased)
numberOfTeaPurchased = int(input("Enter the number of tea purchased (default: 2): ") or teaPurchased)
numberOfCookiesPurchased = int(input("Enter the number of cookies purchased (default: 1): ") or cookiesPurchased)
priceOfFirstItem = float(input("Enter the price of the first item (default: 5): ") or priceCoffee)
priceOfSecondItem = float(input("Enter the price of the second item (default: 4): ") or priceMuffins)
priceOfThirdItem = float(input("Enter the price of the third item (default: 6): ") or priceTea)
priceOfFourthItem = float(input("Enter the price of the fourth item (default: 3): ") or priceCookies)
priceOfTax = float(input("Enter the tax amount (default: 0.78): ") or priceTax)

# Calculate total cost
totalCost = (numberOfCoffeesPurchased * priceOfFirstItem) + (numberOfMuffinsPurchased * priceOfSecondItem) + (numberOfTeaPurchased * priceOfThirdItem) + (numberOfCookiesPurchased * priceOfFourthItem)
totalCostWithTax = totalCost + priceTax

# Display the receipt
print('**************************')
print('My Coffee and Muffin Shop')
print('Number of Coffees Bought:', numberOfCoffeesPurchased)
print('Number of Muffins Bought:', numberOfMuffinsPurchased)
print('Number of Tea Bought:', numberOfTeaPurchased)
print('Number of Cookies Bought:', numberOfCookiesPurchased)
print('**************************')
print('**************************')
print('My Coffee and Muffin Shop Receipt')
print(numberOfCoffeesPurchased, 'Coffee at', priceOfFirstItem, 'each:', numberOfCoffeesPurchased * priceOfFirstItem)
print(numberOfMuffinsPurchased, 'Muffins at', priceOfSecondItem, 'each:', numberOfMuffinsPurchased * priceOfSecondItem)
print(numberOfTeaPurchased, 'Tea at', priceOfThirdItem, 'each:', numberOfTeaPurchased * priceOfThirdItem)
print(numberOfCookiesPurchased, 'Cookies at', priceOfFourthItem, 'each:', numberOfCookiesPurchased * priceOfFourthItem)
print('Tax (6%):', totalCost * priceTax)
print('-----------------')
print('Total Cost:   ', totalCostWithTax)
print ('*************************')
