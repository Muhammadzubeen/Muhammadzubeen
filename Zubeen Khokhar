# J-son
import requests
import json

# BLS Italy API credentials
API_KEY = "YOUR_API_KEY"
API_SECRET = "YOUR_API_SECRET"

# BLS Italy API endpoint
BOOKING_URL = "(https://blsitalypakistan.com/account/account_details)"

# Appointment details
APPOINTMENT_DETAILS = {
    "country": "Pakistan",
    "city": "Islamabad",
    "service": "Italian Visa",
    "date": "2024-08-17",
    "time": "10:00",
    "name": "Muhammad Zubeen",
    "email": "engineerzubeen345@gmail.com",
    "phone": "3349931691",
    "passport_number": "AF5004331",
    "passport_expiry": "2032-01-12"
}

# Set API headers
headers = {
    "Authorization": f"Bearer {API_KEY}",
    "Content-Type": "application/json"
}

# Convert appointment details to JSON
data = json.dumps(APPOINTMENT_DETAILS)

# Send POST request to book appointment
response = requests.post(BOOKING_URL, headers=headers, data=data)

# Check if appointment was booked successfully
if response.status_code == 201:
    print("Appointment booked successfully!")
else:
    print("Error booking appointment:", response.text)
