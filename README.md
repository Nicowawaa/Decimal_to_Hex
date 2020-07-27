# Decimal_to_Hex
Program that converts a decimal value to a hexadecimal value in Python3 


x = input("Enter a decimal value: ")

f = []
L = x
Result = 1;

while (Result>0):
    Remainder = int(x)%16
    
    if Remainder>9:
        if Remainder == 10:
            Remainder = 'A'
            
        elif Remainder == 11:
            Remainder = 'B'
            
        elif Remainder == 12:
            Remainder = 'C'
            
        elif Remainder == 13:
            Remainder = 'D'
            
        elif Remainder == 14:
            Remainder = 'E'
            
        elif Remainder == 15:
            Remainder = 'F'

    f = [Remainder,f]
    
    #print("Remainder",Remainder)
    print("Original Value:", L)
    print ("Hex:",f)
    Result = int(int(x)/16)
    
    if Result == 0:
        break
    x = Result
    #print("Result", Result)
