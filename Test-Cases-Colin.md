# Test Cases -Colin
  
**IDENTIFIER:** TEST-MENU-FILE

**DESCRIPTION:** This test determines if the File menu populates Open File, Save File, Save As, and Quit.

**PRECONDITIONS:** JBefunge is compiled as specified by its readme.

**EXECUTION STEPS:**

    1. Run JBefunge.
    2. Select the File menu item
    3. Observe Open File, Save File, Save As, and Quit listed underneath.

**POSTCONDITIONS:** Open File, Save File, Save As, and Quit are options listed under the File menu. 

---
**IDENTIFIER:** TEST-MENU-COLOR

**DESCRIPTION:** This test determines if the Color menu populates Red, Yellow, Blue, Pink, Green, and Orange.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Select the Color menu item.
    2. Observe Red, Yellow, Blue, Pink, Green, and Orange listed underneath.

**POSTCONDITIONS:** Red, Yellow, Blue, Pink, Green, and Orange are listed under the Color menu. 

---
**IDENTIFIER:** TEST-MENU-OPTIONS

**DESCRIPTION:** This test determines if the Options menu populates Time Program and Check for End Opcode.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Select the Option menu item.
    2. Observe checkable items Time Program and Check for End Opcode.

**POSTCONDITIONS:** Checkable items Time Program and Check for End Opcode are listed under Options. 

---
**IDENTIFIER:** TEST-RUN-SPEED

**DESCRIPTION:** This test determines if the Run button executes with no pauses in exectution.

**PRECONDITIONS:** JBefunge is running, Time Program has been checked, and "HelloWorld.bf" has been opened.

**EXECUTION STEPS:**

    1. Press the Run button.
    2. Record its Time to execute.

**POSTCONDITIONS:** The HelloWorld.bf program should run in under 100,000 microseconds with no pauses in execution.

---
  
**IDENTIFIER:** TEST-WALK-SPEED

**DESCRIPTION:** This test determines if the Walk button executes with a 50 ms pause after each opcode.

**PRECONDITIONS:** JBefunge is running, Time Program has been checked, and HelloWorld.bf has been opened. 

**EXECUTION STEPS:**

    1. Press the Walk button.
    2. Record its Time to execute.

**POSTCONDITIONS:** The HelloWorld.bf program should Walk around 50x longer than its run speed.

---
 
 **IDENTIFIER:** TEST-MOSEY-SPEED

**DESCRIPTION:** This test determines if the Mosey button executes with a 500 ms pause after each opcode.

**PRECONDITIONS:** JBefunge is running, Time Program has been checked, and HelloWorld.bf has been opened. 

**EXECUTION STEPS:**

    1. Press the Mosey button.
    2. Record its Time to execute.

**POSTCONDITIONS:** The HelloWorld.bf program should Mosey around 10x longer than its walk speed.

---
 
**IDENTIFIER:** TEST-TIME-ON

**DESCRIPTION:** This test determines if, when Time program is checked, the total time to execute is 
displayed after running a program.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Open the Options menu, check the "Time program" checkbox.
    2. Run the included FizzBuzz program.
    3. Ensure the time to execute in microseconds is displayed.

**POSTCONDITIONS:** The correct time to execute is displayed after running FizzBuzz.

---
 
 **IDENTIFIER:** TEST-TIME-OFF

**DESCRIPTION:** This test determines if, when Time program is not checked, the total time to execute is not
displayed after running a program.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Open the Options menu, ensure the "Time program" checkbox is empty.
    2. Run the included FizzBuzz program.
    3. Ensure the time to execute in microseconds is not displayed.

**POSTCONDITIONS:** No time to execute in microseconds is displayed.

---
 
 **IDENTIFIER:** TEST-TIME-SWITCH

**DESCRIPTION:** This test is a **Edge Case** that checks for correct execution time if Time Program is selected mid-execution.

**PRECONDITIONS:** JBefunge is running.

**EXECUTION STEPS:**

    1. Open the Options menu, ensure the "Time program" checkbox is empty.
    2. Run the included FizzBuzz program.
    3. Before FizzBuzz finishes execution, open the Options menu and press "Time program"
    3. Observe the time to execute.

**POSTCONDITIONS:** Correct execution time is displayed.

---

**IDENTIFIER:** TEST-BEFUNGE-VALID

**DESCRIPTION:** This test determines if JBefunge can successfully execute a JBefunge-93 program.

**PRECONDITIONS:** JBefunge is running and "HelloWorld.bf" has been opened in the IDE.

**EXECUTION STEPS:**

    1. Press the "Run" button.
    2. Wait for execution to finish.

**POSTCONDITIONS:** The stack is empty and "Hello, World!" is printed in the Output field.

---
 
 **IDENTIFIER:** TEST-BEFUNGE-INVALID

**DESCRIPTION:** This test is an **Edge Case** to determine if JBefunge will run an invalid Java program.

**PRECONDITIONS:** JBefunge is running and a basic Java "Hello, World!" program is entered in the Program Area.
(WARNING: Test will continue to execute indefinitely, will need to be interrupted.)

**EXECUTION STEPS:**

    1. Press the "Run" button.
    2. Observe the Stack and Output textboxes.

**POSTCONDITIONS:** Program continues to execute indefinitely, with nothing displayed in the Stack or Output textboxes.

---
 
 **IDENTIFIER:** TEST-100%-CPU-PERF-EXECUTION-TIME

**DESCRIPTION:** This test determines if a computer with a clock speed over 1.3 GHz can run FizzBuzz.bf in under 30 seconds on Run.

**PRECONDITIONS:** JBefunge is running. FizzBuzz.bf has been opened and Time Program has been checked. Computer's clock speed is over 1.3 GHz.

**EXECUTION STEPS:**

    1. Press the Run button.
    2. Wait for execution to finish.

**POSTCONDITIONS:** Time to execute is under 30 seconds (or 30,000,000 microseconds)

---
 
**IDENTIFIER:** TEST-50%-CPU-PERF-EXECUTION-TIME

**DESCRIPTION:** This test determines if a computer with a clock speed under 1.3 GHz can run FizzBuzz.bf in under 30 seconds on Run.

**PRECONDITIONS:** 

    1. A Windows 10 Virtual Machine set to 50% Execution Cap is running (simulating a 1.2 GHz Machine).
    2. JBefunge is compiled and Running.
    3. FizzBuzz.bf has been opened in JBefunge.

**EXECUTION STEPS:**

    1. Press the Run button.
    2. Wait for execution to finish.

**POSTCONDITIONS:** Time to execute is under 30 seconds (or 30,000,000 microseconds)

---
