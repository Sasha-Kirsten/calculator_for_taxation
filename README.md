# calculator_for_taxation

number_hours_worked = int(input("How many hours worked per week?"))

hourly_pay_rate = float(input("What is the hourly pay rate?"))

gross_pay = number_hours_worked * hourly_pay_rate

count = 0

while count == 0:
        
    tax_rate = float(input("What is the tax rate?"))

    net_pay = gross_pay * (1- tax_rate)

    if tax_rate > 0 and tax_rate < 1:
            
       print("Gross pay (in GBP):", gross_pay)
       print("Net pay (in GBP):", round(net_pay,2))
       count = 1

    else:
    
       print("Please enter tax rate from 0 to 1")
            

