# Checklist: Room Booking Testing

## 1. Positive Scenarios (Happy Path)
- [ ] Book Single, Double, and Suite rooms with valid data for next week (2 nights)
- [ ] Book a room with valid data starting from the current week (3 nights)
- [ ] Verify Price Summary calculation for different duration lengths:
  * Single Room (£100 per night)
  * Double Room (£150 per night)
  * Suite Room (£225 per night)
- [ ] Verify that Cleaning (£25) and Service (£15) fees remain fixed and do not multiply by number of nights.
-  [ ] Verify that changing the booking month or selecting different future dates recalculates the price correctly without system errors.

## 2. Text Fields Validation (Negative Scenarios)
- [ ] Click 'Reserve Now' with all contact fields empty (Verify error messages appear).
- [ ] Input numbers and special characters into 'Firstname' and 'Lastname' fields (e.g., Josh22, Jacob_@1!;)
- [ ] Input invalid email field:
  * Missing '@' symbol (e.g., testmail.com)
  * Missing domain name (e.g., test@)
  * Invalid/overlong top-level domain (e.g., test@mail.cooom)
- [ ] Input alphabetic and special characters into 'Phone' field (Verify it triggers error)
- [ ] Input out-of-boundary length values into 'Phone' field (Less than 11 and more than 20 characters)


