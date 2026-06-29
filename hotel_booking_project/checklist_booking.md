# Checklist: Room Booking Testing

## 1. Positive Scenarios (Happy Path)
- [x] Book Single, Double, and Suite rooms with valid data for next week (2 nights)
- [x] Book a room with valid data starting from the current week (3 nights)
- [x] Verify Price Summary calculation and fixed fees (Cleaning (£25), Service (£15) for different situations:
  * [x] Single Room (£100 per night) -> £240 for 2 nights
  * [x] Double Room (£150 per night) -> £490 for 3 nights
  * [x] Suite Room (£225 per night) -> £940 for 4 nights
- [x] Verify that changing the booking month or selecting different future dates recalculates the price correctly without system errors.

## 2. Text Fields Validation (Negative Scenarios)
- [x] Click 'Reserve Now' with all contact fields empty (Verify error messages appear). `Found Bug #4`
- [ ] Input numbers and special characters into 'Firstname' and 'Lastname' fields (e.g., Josh22, Jacob_@1!;) `Failed` `Bug #5`
- [ ] Input invalid email field:
  * [x] Missing '@' symbol (e.g., testmail.com)
  * [x] Missing domain name (e.g., test@)
  * [ ] Invalid/overlong top-level domain (e.g., test@mail.cooom) `Failed` `Bug #6`
- [ ] Input alphabetic and special characters into 'Phone' field (Verify it triggers error) `Failed` `Bug #7`
- [x] Input out-of-boundary length values into 'Phone' field (Less than 11 and more than 20 characters)

## 3. Date selection & Calendar validation 
- [ ] Try to select past dates on the calendar (Verify that dates before today are disabled)
- [ ] Try to book a room with check-out date prior to check-in date (e.g., Check-in: Today, Check-out: Yesterday)
- [ ] Select an extremely long booking duration (e.g., 45 nights) to verify maximum limit restrictions and price calculation stability. 

