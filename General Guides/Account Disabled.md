## **Issue: Account Disabled**

### **Possible Causes:**
- **Logging in on the account too frequently:** Excessive login attempts may trigger security measures, leading to account disablement.
- **Inactive status set to 0 in the database (PMA):** If the account's status is set to inactive in the database, it might result in the account being disabled.

### **How to Fix:**

#### **For Inactive Status:**
1. Access PhpMyAdmin (PMA).
2. Navigate to the Accounts Table.
3. Locate and select the disabled account.
4. Edit the account details.
5. Set the isActive field to 1 to enable the account.

#### **For Excessive Login Attempts:**
1. Access PhpMyAdmin (PMA).
2. Go to the Accounts Table.
3. Identify the ID of the disabled account.
4. Navigate to the Actions Table.
5. Delete (drop) any actions with ID of 6 associated with the disabled account.
6. This action will remove the excessive login attempts and potentially re-enable the account.
