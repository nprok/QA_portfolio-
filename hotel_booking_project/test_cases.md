## 1. Positive Scenarios (Happy Path)

### TC-001: Verify successful room booking with valid data
**Preconditions:**
* User is on the hotel home page.
* The "Single Room" is available for the selected dates.

| Step # | Action | Expected Result |
| :--- | :--- | :--- |
| **1** | Scroll down to the "Single Room" card and click the "Book Now" button. | Booking form opens, displaying the calendar. |
| **2** | Select check-in and check-out dates for the next week (2 nights). | Total price in "Total" is calculated correctly (£100/night * 2 + £40 fees = £240). |
| **3** | Click "Reserve Now" button | Contact form opens, displaying contact fields. |
| **4** | FIll in the contact fields with valid data: <br>* Firstname: 'Josh' <br>* Lastname: 'Berry' <br>* Email: 'jberr@mail.com' <br>* Phone: 65782537192 | The fields accept the data, and no validation errors or warnings appear. |
| **5** | Click the "Reserve Now" button. | "Booking Confirmed" modal message appears showing the exact selected dates. |

Status: Passed 
