# Test Cases -Ben
  
**IDENTIFIER:** FUN-TEXT-DISPLAY

**DESCRIPTION:** This test verifies that the GUI displays three text boxes labeled 'Program Area', 'Stack', and 'Output'.

**PRECONDITIONS:** JBefunge is compiled as specified by its readme.

**EXECUTION STEPS:** y
    1.The user runs JBefunge

**POSTCONDITIONS:** The JBefunge GUI displayed, showing  three text boxes labeled
'Program Area', 'Stack', and 'Output'respectively. 

---
**IDENTIFIER:** FUN-EDITABLE-PROGRAM-AREA-TEXT-DISPLAY

**DESCRIPTION:** This test verifies that the 'Program Area' text box may be edited by the user. 

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**
    1. Click on the upper-most text box labeled 'Program Area'.
    2. Type the word 'test'.

**POSTCONDITIONS:** Verify that the word 'test' has appeared in the selected
text-box. 

---
**IDENTIFIER:** FUN-UNEDITABLE-PROGRAM-AREA-TEXT-DISPLAY

**DESCRIPTION:** This test verifies that the 'Stack' and 'Output' text boxes cannot
be edited by the user. 

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**
    1. Click on the middle text box labeled 'Stack'.
    2. Type the word 'test'.
    3. Repeat steps 1 and 2 for the lower-most text box labeled 'Output'.

**POSTCONDITIONS:** Verify that the word 'test' has not appeared in neither the
'Stack' nor the 'Output' text boxes. 

---
**IDENTIFIER:** FUN-SAVE-FILE-CREATION

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
**IDENTIFIER:** FUN-SAVE-FILE-UPDATE

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---

**IDENTIFIER:** FUN-SAVE-AS-FILE-CREATION

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
**IDENTIFIER:** FUN-OPEN-FILE

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
**IDENTIFIER:** FUN-OPEN-FILE-CHANGES-GUI-TITLE

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
**IDENTIFIER:** FUN-OPEN-FILE-LOADS-INTO-PROGRAM-AREAD

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
**IDENTIFIER:** FUN-SAVE-FILE 

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
[PAGEBREAK]

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
