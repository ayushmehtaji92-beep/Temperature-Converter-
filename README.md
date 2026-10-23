# Temperature-Converter-
print("=== Temperature Converter ===")
print("1. Celsius to Fahrenheit")
print("2. Fahrenheit to Celsius")
print("3. Celsius to Kelvin")
print("4. Kelvin to Celsius")
print("5. Fahrenheit to Kelvin")
print("6. Kelvin to Fahrenheit")

choice = input("Enter your choice (1-6): ")

temp = float(input("Enter the temperature: "))

if choice == "1":
    result = (temp * 9/5) + 32
    print(f"Temperature: {result:.2f} °F")

elif choice == "2":
    result = (temp - 32) * 5/9
    print(f"Temperature: {result:.2f} °C")

elif choice == "3":
    result = temp + 273.15
    print(f"Temperature: {result:.2f} K")

elif choice == "4":
    result = temp - 273.15
    print(f"Temperature: {result:.2f} °C")

elif choice == "5":
    result = (temp - 32) * 5/9 + 273.15
    print(f"Temperature: {result:.2f} K")

elif choice == "6":
    result = (temp - 273.15) * 9/5 + 32
    print(f"Temperature: {result:.2f} °F")

else:
    print("Invalid choice! Please select 1 to 6.")
