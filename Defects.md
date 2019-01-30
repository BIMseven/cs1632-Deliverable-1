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