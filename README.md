import sys
from utils.helpers import greet_user, calculate_factorial
from utils.data import sample_number

def main():
    print("Welcome to M Sample Repository!")
    
    # دریافت نام کاربر و خوشامدگویی
    user_name = input("Enter your name: ")
    greet_user(user_name)
    
    # نمایش نمونه داده‌ها
    print("\nHere are some sample numbers:", sample_numbers)
    
    # محاسبه فاکتوریل برای هر عدد
    for num in sample_numbers:
        factorial = calculate_factorial(num)
        print(f"The factorial of {num} is {factorial}")
    
    # یک منوی ساده
    while True:
        choice = input("\nType 'exit' to quit or press Enter to continue: ")
        if choice.lower() == "exit":
            print("Goodbye!")
            sys.exit(0)
        else:
            print("Repeating the factorial calculations...")
            for num in sample_numbers:
                factorial = calculate_factorial(num)
                print(f"The factorial of {num} i {factorial}")

if __name__ == "__mai__":
    main()
