FUN-TEXT-DISPLAY - Upon startup, the system shall display a graphical user interface with three textboxes, labeled Program Area, Stack, and Output.  The Program Area textbox shall be user-editable; the other two will never be editable directly by the user.  


FUN-FILE-LOADING - Users shall be able to save their programs using the Save File and Save As functionality.  If a program has not been named yet (either by saving or loading from a previously-named file), then both shall act in the same manner, asking the user to select a name using a File Selection dialog; otherwise, Save File shall simply save the file to the already-selected file.  They may load a file into the GUI by selecting the Open File, at which point the data in the file shall be loaded into the Program Area and the name of the program changed to the name of the file opened.   At all points, the name of the program shall be displayed at the top of the GUI, or "UNTITLED" only if the the program has never been named or opened from a file.




FUN-STEP - The system shall allow the user to step one opcode at a time, appropriately updating the stack and output, by pressing the Step button.

FUN-STOP - When no program is being executed, the Stop button shall be disabled.  When a program is being executed, the Stop button shall be enabled.  Upon clicking the Stop button, the currently running program shall stop execution.



FUN-TRACE - If and only if a program is being executed, the system shall display a cursor on the current opcode indicating that is being executed.  This cursor should start displaying immediately after starting execution of a program on the first opcode, and will do so no matter if started via Run, Walk, Mosey, or Step.  It shall not appear when a program is not being executed.

