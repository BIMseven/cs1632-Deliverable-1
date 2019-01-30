# Test Cases -Ben
  
**IDENTIFIER:** FUN-TEXT-DISPLAY

**DESCRIPTION:** This test verifies that the GUI displays three text boxes labeled 'Program Area', 'Stack', and 'Output'.

**PRECONDITIONS:** JBefunge is compiled as specified by its readme.

**EXECUTION STEPS:** 
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

**DESCRIPTION:** This test verifies that using the 'save file' command under the file
menu on a new, untitled program will create a file of the specified name in the
specified directory.

**PRECONDITIONS:** JBefunge is running with a new, untitled program. The title of the
window reads 'UNTITLED' and the program area is empty.

**EXECUTION STEPS:**
    1. Click on the program area text box, and type "test-text".
    2. Click the file menu and click on "save file". 
    3. Choose a directory (Desktop for example), type a unique file name in the 'File
    Name:' field (save-test for example), and press the "save" button.
    4. Clear the "Program Area" text box.
    5. Click on "open file" under the file menu.
    6. Navigate to directory where the test file was saved, and locate to saved file.
    7. Double-click on the file, opening it.

**POSTCONDITIONS:** 
    The file saved with a unique file name creates a new file in the specified directory.
    Opening this file displays "test-text" in the program area. 

---
**IDENTIFIER:** FUN-SAVE-FILE-UPDATE

**DESCRIPTION:** This test verifies that saving an updated applies any changes to an
existing file.

**PRECONDITIONS:** JBefunge is running with a new, untitled program. The title of the
window reads 'UNTITLED' and the program area is empty.

**EXECUTION STEPS:**
    1. Click on the program area text box, and type "test-text".
    2. Click the file menu and click on "save file". 
    3. Choose a directory (Desktop for example), type a unique file name in the 'File
    Name:' field (save-test for example), and press the "save" button.
    4. Clear the "Program Area" text box, and type "new-stuff".
    5. Repeat step 2.
    6. Close and reopen JBefunge, the title should read "UNTITLED".
    7. Click on "open file" under the file menu.
    8. Navigate to directory where the test file was saved, and locate to saved file.
    9. Double-click on the file, opening it.

**POSTCONDITIONS:** 
    The file saved with a unique file name creates a new file in the specified directory.
    Opening this file displays "new-stuff" in the program area.

---

**IDENTIFIER:** FUN-SAVE-AS-FILE-CREATION

**DESCRIPTION:** This test case verifies that the save as function creates a new file
when given a unique name.

**PRECONDITIONS:** JBefunge is running with a new, untitled program. The title of the
window reads 'UNTITLED' and the program area is empty.

**EXECUTION STEPS:**
    1. Click on the program area text box, and type "test-text".
    2. Click the file menu and click on "save file". 
    3. Choose a directory (Desktop for example), type a unique file name in the 'File
    Name:' field (save-test for example), and press the "save" button.
    4. Clear the "Program Area" text box, and type "new-stuff".
    5. Click on "Save as" under the file menu.
    6. Repeat step 3 with a different file name (save-as-test).
    7. Close and reopen JBefunge, the title should read "UNTITLED".
    8. Click on "open file" under the file menu.
    9. Navigate to directory where the second test file was saved, and locate the saved file.
    10. Double-click on the file, opening it.

**POSTCONDITIONS:** 
    The second file saved with a unique file name creates a new file in the specified directory.
    Opening this file displays "new-stuff" in the program area, and the opened unique file
    name in the title of the window.

---
**IDENTIFIER:** FUN-SAVE-AS-FILE-UPDATE

**DESCRIPTION:** This test case verifies that 

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
