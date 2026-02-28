# flight ticket
flight_no = "AI203"
base_fare = "4500.75"
tax_percent = "5"
seat_numbers = "12A,12B,14C,15D"
is_international = "True"

# Convert base_fare and tax_percent to numeric types
base_fare = float(base_fare)
tax_percent = float(tax_percent)

# Calculate final fare
Final_fare = base_fare + (base_fare*tax_percent / 100)

print("Final Fare for one pssenger:", Final_fare)

# Convert seat number strimng into list
seat_list = seat_numbers.split(",")

print("Seat List:", seat_list)

# Convert list into set
seat_set = set(seat_list)

print("Seat Set:", seat_set)

#Convert is_international into boolean
is_international = is_international == "True"

print("Is international Flight:", is_international)

#Create a flight_summary
flight_summary = {
    "flight_no": flight_no,
    "final_fare": int(Final_fare),
    "seat_numbers": tuple(seat_list)
}

print(flight_summary)
