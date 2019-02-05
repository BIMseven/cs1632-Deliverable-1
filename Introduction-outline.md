* __Introduction__
  * What we tested:
    * File I/O functionality
    * Program Execution
      * Speed
      * Execution Time
    * Editor layout
    * Overall, this test plan offers fairly complete coverage of the requirements and expected behavior.
  * Problems Testing:
    * Testing min execution time was difficult
      * Installing a VM and ensuring it could run a JBefunge program was difficult.
    * Testing run-speed of run/walk/mosey was difficult
      * Simply took a long time
  * Concerns:
    * Tests mentioned above vary based on computer preformance and run in a variable amount of time, causing overall execution time to be inconsistent. In a best-case-scenario, we would be able to run this and average a large sample of run-times. This would take up a large amount of time for testing one requirement, essentially making it infeasible to test. 
    * File I/O produces bugs inconsistently. 