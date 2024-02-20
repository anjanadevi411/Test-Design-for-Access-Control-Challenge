## Test-Design-for-Access-Control-Challenge

<hr>

### Assumptions:
- User roles and permissions are implemented correctly.
- The system allows for creating test users with specific roles.
  
### Test Design: 
#### 1. User Role Verification
#### 2. Access Control for Admin
#### 3. Access Control for Brand Admin
#### 4. Access Control for User
#### 5. Unauthorized Access Attempts
#### 6. Edge Cases and Error Handling
#### 7. Concurrent Access:

### Test cases:
### 1.User Role Verification
- Test 1.1: Verify that Admin, Brand Admin, and User roles are assigned correctly during registration.
- Test 1.2: Verify that changing user roles by the Admin works as expected.
- Test 1.3: Verify that users cannot change their own roles.
  
### 2. Access Control for Admin:
- Test 2.1: Verify that Admin can create, update, and delete all entities (Brands, Product Lists, Products).
- Test 2.2: Verify that Admin can create, update, and delete User accounts with different roles.
- Test 2.3: Verify that Admin can grant and revoke permissions to User accounts.
  
### 3. Access Control for Brand Admin:
- Test 3.1: Verify that Brand Admin can only manage Product Lists and the Brand associated with their role.
- Test 3.2: Verify that Brand Admin cannot access or modify other Brand's entities.
- Test 3.3: Verify that Brand Admin cannot create new Brands or modify Admin accounts.
  
### 4. Access Control for User:
- Test 4.1: Verify that User can only view all entities (Brands, Product Lists, Products).
- Test 4.2: Verify that User cannot create, update, or delete any entity.
- Test 4.3: Verify that User cannot access Admin or Brand Admin functionalities.
  
### 5. Unauthorized Access Attempts:
- Test 5.1: Try to access entities with unauthorized roles (e.g., User trying to create/update/delete a Brand).
- Test 5.2: Try to modify entities that the user shouldn't have access to (e.g., Brand Admin trying to modify another Brand's Product List, products).
  
### 6. Edge Cases and Error Handling:
- Test 6.1: Test access control behavior when dealing with invalid roles, non-existent brands or permission conflicts.
- Test 6.2: Verify error handling for unauthorized access attempts and unexpected scenarios's.
  
### 7. Concurrent Access:
- Test 7.1: Simulate concurrent access from multiple users with different roles and test for potential race conditions or data inconsistencies.
  
### Documentation:
- Each test case will be documented with:
- Description of the scenario
- preconditions
- Steps to execute the test case
- Expected outcome
- actual outcome
- severity

  ##### I have covered a little bit of test secanrios once enter deeply into the software more secanrio's might arise.

  
