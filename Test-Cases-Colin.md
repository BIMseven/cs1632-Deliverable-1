# Test Cases -Colin
  
**IDENTIFIER:** FUN-MENU-FILE

**DESCRIPTION:** This test determines if the File menu populates Open File, Save File, Save As, and Quit.

**PRECONDITIONS:** JBefunge is compiled as specified by its readme.

**EXECUTION STEPS:**

    1. Run JBefunge.
    2. Select the File menu item
    3. Observe Open File, Save File, Save As, and Quit listed underneath.

**POSTCONDITIONS:** Open File, Save File, Save As, and Quit are options listed under the File menu. 

---
**IDENTIFIER:** FUN-MENU-COLOR

**DESCRIPTION:** This test determines if the Color menu populates Red, Yellow, Blue, Pink, Green, and Orange.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Select the Color menu item.
    2. Observe Red, Yellow, Blue, Pink, Green, and Orange listed underneath.

**POSTCONDITIONS:** Red, Yellow, Blue, Pink, Green, and Orange are listed under the Color menu. 

---
**IDENTIFIER:** FUN-MENU-OPTIONS

**DESCRIPTION:** This test determines if the Options menu populates Time Program and Check for End Opcode.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Select the Option menu item.
    2. Observe checkable items Time Program and Check for End Opcode.

**POSTCONDITIONS:** Checkable items Time Program and Check for End Opcode are listed under Options. 

---
**IDENTIFIER:** FUN-RUN-SPEED

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
  
**IDENTIFIER:** FUN-WALK-SPEED

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
 
 **IDENTIFIER:** FUN-MOSEY-SPEED

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
 
**IDENTIFIER:** FUN-TIME-ON

**DESCRIPTION:** This test determines if, when Time program is checked, the total time to execute is 
displayed after running a program.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Open the Options menu, check the "Time program" checkbox.
    2. Run the included FizzBuzz program.
    3. Ensure the time to execute in microseconds is displayed.

**POSTCONDITIONS:** The correct time to execute is displayed after running FizzBuzz.

---
 
 **IDENTIFIER:** FUN-TIME-OFF

**DESCRIPTION:** This test determines if, when Time program is not checked, the total time to execute is not
displayed after running a program.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Open the Options menu, ensure the "Time program" checkbox is empty.
    2. Run the included FizzBuzz program.
    3. Ensure the time to execute in microseconds is not displayed.

**POSTCONDITIONS:** No time to execute in microseconds is displayed.

---

**IDENTIFIER:** FUN-BEFUNGE-VALID

**DESCRIPTION:** This test determines if JBefunge can successfully execute a JBefunge-93 program.

**PRECONDITIONS:** JBefunge is running and "HelloWorld.bf" has been opened in the IDE.

**EXECUTION STEPS:**

    1. Press the "Run" button.
    2. Wait for execution to finish.

**POSTCONDITIONS:** The stack is empty and "Hello, World!" is printed in the Output field.

---
 
 **IDENTIFIER:** FUN-BEFUNGE-INVALID

**DESCRIPTION:** This test is an Edge Case to determine if JBefunge will run an invalid Java program.

**PRECONDITIONS:** JBefunge is running and a basic Java "Hello, World!" program is entered in the Program Area.
(WARNING: Test will continue to execute indefinitely, will need to be interrupted.)

**EXECUTION STEPS:**

    1. Press the "Run" button.
    2. Observe the Stack and Output textboxes.

**POSTCONDITIONS:** Program continues to execute indefinitely, with nothing displayed in the Stack or Output textboxes.

---
 
 **IDENTIFIER:** PERF-EXECUTION-TIME

**DESCRIPTION:** 

**PRECONDITIONS:** 

**EXECUTION STEPS:**
    1.

**POSTCONDITIONS:** 

---
 
 
