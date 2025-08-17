#Functions
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = (discount_percent/100)*price
        new_price = price - discount_amount
        return new_price
    
    else: 
        return price
    
price = int(input("Enter the original price here:"))
discount_percent =int(input("Enter the discounted percent here"))
final_price = calculate_discount(price, discount_percent)
print(f"Your final price is {final_price}")
