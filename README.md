feet_per_gallon = 112
labor_hours = 8
labor_charge = 35
def setPaint(getSpace,gallonPaint):
    gallonPaint=getSpace/feet_per_gallon
    return gallonPaint
def setHours(gallonPaint,hourLabor):
    hourLabor=gallonPaint*labor_hours
    return hourLabor
def setPaintcharge(gallonPaint,pricePaint):
    costPaint=gallonPaint*getPrice
    return costPaint
def setLaborCharge(hourLabor,costLabor):
    costLabor=hourLabor*labor_charge
    return setLaborCharge
def showIncome(gallonPaint,hourLabor,costPaint,costLabor):
    showIncome=costPaint+costLabor
    return showIncome
def main():
    getSpace=int(input("Enter wall space in square feet:"))
    getPrice=float(input("Enter paint price per gallon:"))
    gallonPaint=setPaint(getSpace,gallonPaint)
    hourLabor=setHours(gallonPaint,hourLabor)
    costPaint=setPaintcharge(gallonPaint,pricePaint)
    costLabor=setLaborCharge(hourLabor,costLabor)
    showincome=showIncome(gallonPaint,hourLabor,costPaint,costLabor)
    print("Gallons of paint:",+str(gallonPaint))
    print("Hours of labor:",+str(hourLabor))
    print("Paint charge:",+str(costPaint))
    print("Labor charge:",+str(costLabor))
    print("Total cost:",+str(showIncome))
if __name__ == '__main__':
    main()
    
