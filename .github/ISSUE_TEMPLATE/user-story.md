---
name: "User Story"
about: "Create a user story for a feature or task"
title: "[User Story] Money Transfer Feature"
labels: ["user story"]
assignees: []

---

**As a** registered bank user  
**I need** the ability to transfer money to another account  
**So that** I can send funds conveniently without visiting the bank  

---

### 📋 Details and Assumptions
* User must be logged in to initiate a transfer  
* Transfers can only be made to saved beneficiary accounts  
* A confirmation email is sent after each successful transaction  
* The maximum transfer limit per day is ₹1,00,000  

---

### ✅ Acceptance Criteria (Gherkin format)

```gherkin
Given the user is logged in and on the transfer page  
When the user selects a beneficiary and enters a valid amount within the limit  
Then the transfer is processed and a confirmation message is displayed  

Given the user tries to transfer an amount exceeding the daily limit  
When they submit the form  
Then an error message is shown indicating the limit has been exceeded  
