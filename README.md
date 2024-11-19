import calendar

# Function to display the calendar
def display_calendar(year, month):
    # Create a plain text calendar for the given year and month
    cal = calendar.month(year, month)
    print(cal)

# Input from user for year and month
def main():
    try:
        year = int(input("Enter year (e.g., 2024): "))
        month = int(input("Enter month (1-12): "))

        # Validate the month
        if month < 1 or month > 12:
            print("Invalid month! Please enter a month between 1 and 12.")
        else:
            # Display the calendar for the given year and month
            display_calendar(year, month)
    except ValueError:
        print("Invalid input! Please enter a valid number.")

# Run the program
if __name__ == "__main__":
    main()
