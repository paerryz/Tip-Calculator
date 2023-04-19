# Tip-Calculator

#If the bill was $150.00, split between 5 people, with 12% tip. 

#Each person should pay (150.00 / 5) * 1.12 = 33.6
#Format the result to 2 decimal places = 33.60


------------------------------------------------------------------------
bill = float(input("How much is the total bill? $"))
tip = int(input("What percentage do you want to give? 10, 12, or 15? "))
people = int(input("How many people to split the bill? "))

tip_as_percent = tip / 100
bill_with_tip = tip_as_percent * bill
total_bill =  bill_with_tip + bill

final_amount = round(total_bill / people, 2)
final_amount = "{:.2f}".format(final_amount) 
print(f"Each person should pay: ${final_amount}")
