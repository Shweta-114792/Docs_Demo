# Understanding Re-run failed Test Case Feature and Capbilities

### Feature Purpose

In test automation, failures may occur due to various transient reasons such as:

* Temporary environmental issues (e.g., network lag)
* Backend service unavailability
* UI loading delays
* Third-party API latency

Often, these failures are not due to issues in the application under test, but rather external or random factors. This feature allows such failed test cases to be automatically retried, improving the overall pass rate without manual intervention.

### Capabilities

* Re-run of Failed Test Cases\
  Only the test cases that failed in the last execution are rerun. The passed test cases are not run again.
* Configurable Re-run Count (Up to 5 Attempts)\
  The number of times a failed test case should be retried can be set by the user. The maximum allowed reruns are 5.
* Updated Execution Report with Final Results\
  After the reruns, the execution report is updated to show the latest result of each test case.
* E2E Test Cases Treated as One Unit\
  For End-to-End (E2E) test cases, if any step fails, the entire E2E test case will be rerun as one unit.
