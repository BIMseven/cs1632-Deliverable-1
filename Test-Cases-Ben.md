# Test Cases -Ben
  
    IDENTIFIER: FUN-TEXT-DISPLAY

    DESCRIPTION:
        This test verifies that the GUI displays three text boxes labeled 'Program     Area', 'Stack', and 'Output'.

    PRECONDITIONS:
        JBefunge is compiled as specified by its readme.

    EXECUTION STEPS:  
        1.The user runs JBefunge

    POSTCONDITIONS: 
        The JBefunge GUI displayed, showing  three text boxes labeled 'Program Area', 'Stack', and 'Output'respectively. 

---
    IDENTIFIER:  FUN-EDITABLE-PROGRAM-AREA-TEXT-DISPLAY

    DESCRIPTION:  This test verifies that the 'Program Area' text box may be edited by the   user. 

    PRECONDITIONS:  JBefunge is running.

    EXECUTION STEPS: 
        1. Click on the upper-most text box labeled 'Program Area'.
        2. Type the word 'test'.

    POSTCONDITIONS:  Verify that the word 'test' has appeared in the selected
    text-box. 

---
    IDENTIFIER:  FUN-UNEDITABLE-PROGRAM-AREA-TEXT-DISPLAY

    DESCRIPTION:  This test verifies that the 'Stack' and 'Output' text boxes cannot
    be edited by the user. 

    PRECONDITIONS:  JBefunge is running.

    EXECUTION STEPS: 
        1. Click on the middle text box labeled 'Stack'.
        2. Type the word 'test'.
        3. Repeat steps 1 and 2 for the lower-most text box labeled 'Output'.

    POSTCONDITIONS:  Verify that the word 'test' has not appeared in neither the
    'Stack' nor the 'Output' text boxes. 

---
    IDENTIFIER:  FUN-SAVE-FILE-CREATION

    DESCRIPTION:  This test verifies that using the 'save file' command under the file
    menu on a new, untitled program will create a file of the specified name in the
    specified directory.

    PRECONDITIONS:  JBefunge is running with a new, untitled program. The title of the
    window reads 'UNTITLED' and the program area is empty.

    EXECUTION STEPS: 
        1. Click on the program area text box, and type "test-text".
        2. Click the file menu and click on "save file". 
        3. Choose a directory (Desktop for example), type a unique file name in the 'File
        Name:' field (save-test for example), and press the "save" button.
        4. Clear the "Program Area" text box.
        5. Click on "open file" under the file menu.
        6. Navigate to directory where the test file was saved, and locate to saved file.
        7. Double-click on the file, opening it.

    POSTCONDITIONS:  
        The file saved with a unique file name creates a new file in the specified directory.
        Opening this file displays "test-text" in the program area. 

---
    IDENTIFIER:  FUN-SAVE-FILE-UPDATE

    DESCRIPTION:  This test verifies that saving an updated file applies any changes to an
    existing file.

    PRECONDITIONS:  JBefunge is running with a new, untitled program. The title of the
    window reads 'UNTITLED' and the program area is empty.

    EXECUTION STEPS: 
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

    POSTCONDITIONS:  
        The file saved with a unique file name creates a new file in the specified directory.
        Opening this file displays "new-stuff" in the program area.

---

    IDENTIFIER:  FUN-SAVE-AS-FILE-CREATION

    DESCRIPTION:  This test case verifies that the save as function creates a new file
    when given a unique name.

    PRECONDITIONS:  JBefunge is running with a new, untitled program. The title of the
    window reads 'UNTITLED' and the program area is empty.

    EXECUTION STEPS: 
        1. Click on the program area text box, and type "test-text".
        2. Click the file menu and click on "save file". 
        3. Choose a directory (Desktop for example), type a unique file name in the 'File
        Name:' field (save-test for example), and press the "save" button.
        4. Clear the "Program Area" text box, and type "new-stuff".
        5. Click on "Save as" under the file menu.
        6. Repeat step 3 with a different file name (save-as-test).
        7. Close and reopen JBefunge, the title should read "UNTITLED".
        8. Click on "open file" under the file menu.
        9. Navigate to directory where the second test file was saved, and locate the saved     file.
        10. Double-click on the file, opening it.

    POSTCONDITIONS:  
        The second file saved with a unique file name creates a new file in the specified   directory.
        Opening this file displays "new-stuff" in the program area, and the opened unique file
        name in the title of the window.

---
    IDENTIFIER:  FUN-SAVE-AS-FILE-UPDATE

    DESCRIPTION:  This test case verifies that the save as function updates or
    overwrites a specified.  

    PRECONDITIONS:  JBefunge is running with a new, untitled program. The title of the
    window reads 'UNTITLED' and the program area is empty.

    EXECUTION STEPS: 
        1. Click on the program area text box, and type "test-text".
        2. Click the file menu and click on "save file". 
        3. Choose a directory (Desktop for example), type a unique file name in the 'File
        Name:' field (save-as-test for example), and press the "save" button.
        4. Clear the "Program Area" text box, and type "new-stuff".
        5. Click on "Save as" under the file menu.
        6. Repeat step 3.
        7. Close and reopen JBefunge, the title should read "UNTITLED".
        8. Click on "open file" under the file menu.
        9. Navigate to directory where the file was saved, and locate the saved file.
        10. Double-click on the file, opening it.

    POSTCONDITIONS:  
        Opening this file displays "new-stuff" in the program area, and the file
        name in the title of the window.

---
    IDENTIFIER:  FUN-OPEN-FILE-TEXT-LOADS-INTO-PROGRAM-AREA

    DESCRIPTION:  This test verifies that the open file function properly displays the
    text 

    PRECONDITIONS:  JBefunge is running with no program selected, the title reads
    "UNTITLED", and a JBEFUNGE file named "open-test" with a
    body of "test" already exists.

    EXECUTION STEPS: 
        1. Click on the program area text box, and type "removed-text".
        2. Click on "open file" under the file menu.
        3. Navigate to directory where "open-test" exists, and locate "open-test".
        4. Double-click on the file, opening it.

    POSTCONDITIONS:  
        "removed-text" is replaced in the program area

---
    IDENTIFIER:  FUN-OPEN-FILE-CHANGES-GUI-TITLE

    DESCRIPTION:  JBefunge is running with no program selected, the title reads
    "UNTITLED", and a JBEFUNGE file named "open-test" with a
    body of "test" already exists.

    PRECONDITIONS:  JBefunge is running with no program selected, the title reads
    "UNTITLED", and a JBEFUNGE file named "open-test" with a
    body of "test" already exists.

    EXECUTION STEPS: 
        1. Click on "open file" under the file menu.
        2. Navigate to directory where "open-test" exists, and locate "open-test".
        3. Double-click on the file, opening it.

    POSTCONDITIONS:  
       The title of the window is changed from "UNTITLED" to "open-test".

---

    IDENTIFIER:  FUN-OPEN-FILE-LOADS-INTO-PROGRAM-AREA-FROM-OPENED-FILE

    DESCRIPTION:  This test verifies that opening a file while a file already is
    opened updates the program area properly.

    PRECONDITIONS:  JBefunge is running with some file "open-test-1" opened. The title reads
    "open-test-1", and the program area reads "failure". A JBefunge file named "open-test-2"    with a
    body of "success" already exists.

    EXECUTION STEPS: 
        1. Click on "open file" under the file menu.
        2. Navigate to directory where "open-test-2" exists, and open "open-test-2".

    POSTCONDITIONS:  
       The program area reads "success".

---
    IDENTIFIER:  FUN-OPEN-FILE-UPDATES-WINDOW-TITLE-FROM-OPENED-FILE

    DESCRIPTION:  This test verifies that opening a file while a file already is
    opened updates the JBefunge window properly.

    PRECONDITIONS:  JBefunge is running with some file "open-test-fail" opened. The title    reads
    "open-test-fail", and a JBefunge file named "open-test-success" already exists.

    EXECUTION STEPS: 
        1. Click on "open file" under the file menu.
        2. Navigate to directory where "open-test-success" exists, and open "open-test-success".

    POSTCONDITIONS:  
       The title of the JBefunge window reads "open-test-success".

---
    IDENTIFIER: TEST-STEP-OPERATION-MOVEMENT
    DESCRIPTION:
        Ensures that pressing step executes one operation each press.
    PRECONDITIONS:
        JBefunge is running without a file opened.
    EXECUTION STEPS: 
        1. Enter "1234+$" into the Program Area.
        2. Click "Step" 5 times.
    POSTCONDITIONS:  
        The Stack text area displays "[1,2,7]".
---
    IDENTIFIER:  TEST-STEP-STACK-UPDATE
    DESCRIPTION:  
        Verifies that Step updates the Stack appropriately
    PRECONDITIONS:
        JBefunge is running without a file opened.
    EXECUTION STEPS: 
        1. Enter "1." into the Program Area.
        2. Click "Step" once.
    POSTCONDITIONS:  
        The Stack area displays "[1]".
---
    IDENTIFIER:  TEST-STEP-OUTPUT-UPDATE
    DESCRIPTION:  
        Verifies that Step updates the Output text box appropriately.
    PRECONDITIONS:
        JBefunge is running without a file opened.
    EXECUTION STEPS: 
        1. Enter "1." into the Program Area.
        2. Click Step twice.
    POSTCONDITIONS:  
        The Output area displays "1".
---

    IDENTIFIER:  TEST-STEP-CURSOR-DISPLAY

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

---
    IDENTIFIER:  FUN-STOP-DISABLES-STOP

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

---
    IDENTIFIER:  FUN-STEP-ENABLES-STOP-BUTTON

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

---
    IDENTIFIER:  FUN-WALK-ENABLES-STOP-BUTTON

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

---
    IDENTIFIER:  FUN-MOSEY-ENABLES-STOP-BUTTON

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

---
    IDENTIFIER:  FUN-RUN-ENABLES-STOP-BUTTON

    DESCRIPTION:  

    PRECONDITIONS:  

    EXECUTION STEPS: 
        1.

    POSTCONDITIONS:  

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
