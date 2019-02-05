# Defects

    SUMMARY: FUN-OPEN-FILE-DOES-NOT-UPDATE-PROGRAM-AREA
    DESCRIPTION: 
        Running command 'Open File' does not update the text inside of the program-area text box.
    REPRODUCTION STEPS:
        1. Run JBefunge.
        2. Type text 'hello world' into the program area.
        3. Save the file as 'test-1'.
        4. Clear the program area and use save as 'test-2-no-text'.
        5. Close and re-launch JBefunge.
        6. Open 'test-1', which should display 'hello world' in the program area.
        7. Open 'test-2-no-text'.
    EXPECTED BEHAVIOR: Program area should be empty.
    OBSERVED BEHAVIOR: Program still displays 'hello world'.
    SEVERITY: Critical
    IMPACT:Blocking
---
    SUMMARY: FUN-TRACE-NO-CURSOR-ON-FIRST-STEP
    DESCRIPTION: 
        Step does not make the yellow cursor appear if it is the first opcode in the program.
    REPRODUCTION STEPS:
        1. Run JBefunge, an "UNTITLED" new file is open 
        2. Enter "1." into the Program Area.
        3. Click Step.
    EXPECTED BEHAVIOR: Cursor should appear on "1"
    OBSERVED BEHAVIOR: No cursor appears.
    SEVERITY: Minor ??
    IMPACT:??
---
    SUMMARY: PERF-EXECUTUTION-TIME-OVER-30-SECONDS
    DESCRIPTION: 
        UNDER-1.3-PERF-EXECUTION-TIME fails to run FizzBuzz.bf in under 30 seconds
    REPRODUCTION STEPS:
        1. Initialize a Windows 10 Virtual Machine with a 50% Execution Cap.
        2. Install JDK and compile JBefunge, then run JBefunge.
        2. Open File, select FizzBuzz.bf.
        3. Check the Time Program checkbox.
        3. Press Run, wait for execution time pop-up.
    EXPECTED BEHAVIOR: Program finishes execution in under 30,000,000 microseconds.
    OBSERVED BEHAVIOR: Program finished execution in 78,968,914 microseconds on the Virtual Machine.
    SEVERITY: Trivial
    IMPACT: Users with under-powered machines will experience longer wait times for executions of programs.
