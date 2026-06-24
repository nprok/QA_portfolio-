# Checklist: Contact Us Form Testing

## 1. Positive Scenarios
- [x] Submit the form with all fields filled with valid data
- [x] Verify that the success message ("Thanks for getting in touch") is displayed
- [x] Submit the form with the minimum allowed character length in text fields (Subject 5, Phone 11, Message 20)

## 2. Text Fields Validation (Name, Subject, Description)
- [x] Submit the form with empty mandatory fields (verify error messages) `Found Bug #1`
- [x] Input special characters and numbers into the 'Name' field (e.g., `John123`, `John_#`)
- [x] Input extremely long text into 'Subject' and 'Description' fields (boundary testing & layout check)

## 3. Email Field Validation
- [x] Input an invalid email format missing the `@` symbol (e.g., `test-email.com`)
- [ ] Input invalid email format (missing domain e.g., 'testmail@mail') `FAILED` `Bug #2`

## 4. Phone Field Validation
- [ ] Input letters and special characters instead of numbers into the 'Phone' field (verify input restriction) `FAILED` `Bug #3`
- [x] Input an incomplete/too short phone number (e.g., 3-5 digits)
- [x] Input a valid phone number format with standard separators (e.g., `+1 123-45-67` or `123-456-7890`)
