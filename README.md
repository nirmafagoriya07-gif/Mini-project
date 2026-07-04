balance = 5000

while True:
    
    print("~~~ATM~~~")
    print("1. Check balance")
    print("2. Deposit")
    print("3. Withdraw")
    print("4. Exit")
    
    choice = int(input("enter a number              : "))
    if choice == 1:
        print(f"""your curent balance          is {balance}""")
        
    elif choice == 2:
        Deposit = int(input("enter             deposit ammount is : "))
        ammount = balance + Deposit
        print(f"""you deposit                  {Deposit} rupees \nNow current         ammount is {ammount}""")
        
    elif choice == 3:
        Withdraw = int(input("enter            withdraw ammount is : "))
        if Withdraw <= balance:
            print(f"""you withdraw                 {Withdraw} rupees \nNow                current balance is                     {ammount - Withdraw}""")
        else:
            print("not found")
            
    elif choice == 4:
        print("""Thanku have a good            day !""")
        break
        
    else:
        print("""invalid choice try              again """)
        
