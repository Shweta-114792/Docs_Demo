# Best Practices for Re-running Failed Test Case

### **Best Practices to use Re-Run Failed Test Cases feature in Avo Assure:**

**Usage & Scope**

* Use re-run mainly for failures that happen randomly (e.g., network delays or UI slowness)

**Failure Analysis**

* After re-runs, check the client logs to identify the actual reason for the failure

**Configuration**

* Avoid setting a high re-run count for test cases that consistently fail — fix the problem instead

**Reliability**

* Combine re-run with features like **Wait actions** and **On Failure** to improve stability in execution
