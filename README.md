# Female-Macro-Calculator
Calculates maintenance calories for females
#determine ideal calories
#multiply by set percentages
#Finally, divide your calorie amounts by its calorie-per-gram number.
#inputs weight and height
#basal metabolic rate female w * 4.35 h *4.7 sum them and * by 655
#sed = 1.2  lighlt active 1.375 m active 1.55 v active 1.725
# basal metabolo * life style = calories


w = int(input("Hello, What is your weight in lbs?"))
h = float(input("Thanks, what is your height in feet.inches?"))
BMR = ((w*4.35) + (h*4.7)) + 655
al = str(input("What is your activity level?: Sed, Light Active, Active, or Highly Active?"))

if al == "Sed":
    al = 1.7
elif al == "Light Active":
    al = 1.375
elif al == "Active":
    al = 1.55
elif al == "Highly Active":
    al = 1.725
else:
    print("Invalid Activity Level")

calories = BMR * al

print("Your Maintanence Caloreis are:" + str(calories))
