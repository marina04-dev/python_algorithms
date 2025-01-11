# This program takes numbers as inputs and stores them in  different lists whether they are odd or even numbers with inputs check
evenNumbers = []
oddNumbers = []

choice = "i"

while (choice != "q"):
    if choice == " " or choice.isdigit() == True:
        print("Please enter i for insert, d for delete or q for exit! ")
        continue
    else:
        # Insert a number choice
        if choice == "i":
            number =input("Please enter a number: ").strip()
            if number.isdigit():
                number = int(number)
                if number%2==0:
                    evenNumbers.append(number)
                    evenNumbers.sort()
                    evenNumbers.reverse()
                    print("The ordered list is: ",evenNumbers)
                elif number%2!=0:
                    oddNumbers.append(number)
                    oddNumbers.sort()
                    oddNumbers.reverse()
                    print("The ordered list is: ",oddNumbers)
            else:
                print("Wrong input!Please enter only digits!")
            
            
        # Delete choice
        elif choice == "d":
            number =input("Please enter a number: ").strip()
            if number.isdigit():
                number = int(number)
                if number in evenNumbers or number in oddNumbers:
                    if number%2==0:
                        for idex,num in enumerate(evenNumbers):
                            if number==num:
                                evenNumbers.pop(index)
                            print("The ordered list is: ",evenNumbers)
                    elif number%2!=0:
                        for index,num in enumerate(oddNumbers):
                            if number==num:
                                oddNumbers.pop(index)
                            print("The ordered list is: ",oddNumbers)
                else:
                    print(f"Number {number} does not exist in either odd or even numbers list")
                    break
            else:
                print("Wrong input!Please enter only digits!")
                continue
            
        # Exit choice
        elif choice == "q":
            break
    choice=input("Press i to insert new value, d to delete a value or q to exit: ").lower().strip()
print("Thank you")
                
    
