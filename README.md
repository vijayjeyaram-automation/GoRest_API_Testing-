# GoRest API Testing - Postman Collection

This Postman collection includes API tests based on the public API documentation at https://gorest.co.in.

## Requirements

- Postman installed (desktop app recommended)
- A valid GoRest Access Token (for POST request)

---

## Test Scenarios

### Scenario 1: Create a New User
"Endpoint": POST https://gorest.co.in/public/v2/users  
"Description": Creates a new user by providing name, gender, email, and status.  
"Validation": Verifies that the id returned in the response is numeric.

> Requires Bearer Token (Authorization header)

---

### Scenario 2: Validate First User Status
"Endpoint": GET https://gorest.co.in/public/v2/users  
"Description": Fetches all users and validates that the status of the "first user" is either "active" or "inactive".

---

## How to Run the Tests

1. Open Postman
2. Go to the "Collections" tab (left panel)
3. Click "Import" and upload the file:  
   GoRest_API_Tests.postman_collection.json
4. Open the collection → Click "Run Collection"
5. Set your Bearer Token for authorization in the Authorization tab of the POST request
6. Run the collection using the "Collection Runner"
7. Verify test results under the "Test Results" tab

---

## Files Included

- GoRest_API_Tests.postman_collection.json – The exported Postman collection
- README.txt – Instructions for importing and running the tests

---

Created by: Vijayakumar Jeyaram
