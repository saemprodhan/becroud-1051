# becroud-1051
Taxes
salary = float(input())
def calculate_tax(salary):
    tax = 0.0
    if salary <= 2000.00:
        return "Isento"
    if salary > 4500.00:
        tax += (salary - 4500.00) * 0.28
        salary = 4500.00
    if salary > 3000.00:
        tax += (salary - 3000.00) * 0.18
        salary = 3000.00
    if salary > 2000.00:
        tax += (salary - 2000.00) * 0.08
    return f"R$ {tax:.2f}"
print(calculate_tax(salary))
