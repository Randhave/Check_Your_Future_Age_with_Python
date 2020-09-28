# Check_Your_Future_Age_with_Python
def future_Age() :
    
    ageYear = int(input("What is your age or year :"))
    isAge = False
    isYear = False
    if len(str(ageYear)) == int(4) :
        isYear = True
    else :
        isAge = True
 
    if (ageYear < 1990 and isYear) :
     print("You are oldest person and become alive🙄\n")
     exit ()
     
    if (ageYear > 2020) :
        print("You are not Born 😶😶\n")
        exit ()
 
    if (isAge):
       ageYear = 2020 - ageYear

    print(f"You complete 100 year in {ageYear + 100}\n")

    futureAge = int(input("Enter the Year if you want check what is age in Year :" ))
    print(f"You will be in {futureAge - ageYear} year old in {ageYear}\n")
    recheck = str(input("\nYou want to recheck your Age :" ))
    if recheck == 'Y':
        future_Age()
    else  :
        exit ()     
           
future_Age()
