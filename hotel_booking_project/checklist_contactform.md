# Checklist: Contact Us Form Testing

## 1. Positive Scenarios
- [x] Submit the form with all fields filled with valid data
- [ ] Verify that the success message ("Thanks for getting in touch") is displayed
- [ ] Submit the form with the minimum allowed character length in text fields

## 2. Text Fields Validation (Name, Subject, Description)
- [ ] Submit the form with empty mandatory fields (verify error messages)
- [ ] Input special characters and numbers into the 'Name' field (e.g., `John123`, `John_#`)
- [ ] Input extremely long text into 'Subject' and 'Description' fields (boundary testing & layout check)

## 3. Email Field Validation
- [ ] Input an invalid email format missing the `@` symbol (e.g., `test-email.com`)
- [ ] Input an invalid email format missing the domain part (e.g., `test@`)
- [ ] Input a valid email with an uncommon domain extension (e.g., `user@hotel.testing`)

## 4. Phone Field Validation
- [ ] Input letters and special characters instead of numbers into the 'Phone' field (verify input restriction)
- [ ] Input an incomplete/too short phone number (e.g., 3-5 digits)
- [ ] Input a valid phone number format with standard separators (e.g., `+7 (999) 123-45-67` or `123-456-7890`)
