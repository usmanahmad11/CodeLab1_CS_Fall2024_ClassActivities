
# Real-Life Scenarios for If-Else, Elif, and Nested If-Else in Python

## 1. Restaurant Order Discount (if-else)
**Scenario:**  
A customer is ordering food from a restaurant. If the total bill exceeds £50, they get a 10% discount. Write a program to calculate the final bill after applying the discount if applicable.

**Instructions:**
1. Ask the user to input the total bill amount.
2. Use an `if-else` structure to check if the total is more than £50.
3. If it is, apply the 10% discount and print the new total.
4. If not, print the total as is.



---

## 2. Movie Ticket Price (if-elif-else)
**Scenario:**  
A cinema charges different ticket prices based on age:
- Children (0-12 years): £5
- Teenagers (13-17 years): £7
- Adults (18-64 years): £10
- Seniors (65+ years): £6

Write a program to calculate the price of a movie ticket based on the person's age.

**Instructions:**
1. Ask the user to input their age.
2. Use an `if-elif-else` structure to determine the price of the ticket.
3. Display the appropriate ticket price.


## 3. Bank Withdrawal (Nested if-else)
**Scenario:**  
A customer is withdrawing money from their bank account. The withdrawal is only allowed if the account balance is sufficient. If the balance is above £1000, they get a VIP customer message. If the balance is below £100, they get a low-balance warning.

**Instructions:**
1. Ask the user to input their account balance and the amount they want to withdraw.
2. First check if the withdrawal amount is less than or equal to the balance.
3. If the withdrawal is allowed, print the remaining balance.
4. If the balance is more than £1000 after withdrawal, print a VIP message.
5. If the balance is less than £100, print a low-balance warning.




## 4. Weather and Outfit Selection (if-elif-else)
**Scenario:**  
Based on the weather forecast, suggest an outfit:
- If it’s sunny and above 25°C, suggest wearing shorts and sunglasses.
- If it’s rainy, suggest carrying an umbrella.
- If it’s cold (below 10°C), suggest wearing a jacket.
- If it's cloudy but not rainy, suggest wearing light clothes.

**Instructions:**
1. Ask the user to input the weather condition and temperature.
2. Use an `if-elif-else` structure to suggest the appropriate outfit.



## 5. Password Validation (Nested if-else)
**Scenario:**  
A system requires a password to be between 8-16 characters long and contain both letters and numbers. Write a program that checks if a password is valid.

**Instructions:**
1. Ask the user to input a password.
2. Use nested `if-else` statements to check:
   - If the length is between 8-16 characters.
   - If it contains both letters and numbers.
3. Print whether the password is valid or not.

