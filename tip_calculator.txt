print("Welcome to the tip calculator!")

#user inputs

bill = float(input("What was your total bill? $"))
tip = int(input("What percentage tip would like to give? 10, 12, or 15? "))
split = int(input("How many people are splitting the bill? "))

#variables

tip_total = bill * (tip / 100)
final_total = (bill + tip_total) / split
final_split = round(final_total, 2)
final_split = "{:.2f}".format(final_total) 

#Print results

print(f"Each person should pay: ${final_split}")
