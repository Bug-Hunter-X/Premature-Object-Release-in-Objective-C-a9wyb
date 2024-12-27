# Premature Object Release in Objective-C
This repository demonstrates a common error in Objective-C's manual memory management: the premature release of objects.  The `bug.m` file contains code that incorrectly releases an object before it's no longer needed, leading to a crash. The solution, provided in `bugSolution.m`, demonstrates proper memory management techniques to avoid this issue. This is especially relevant for developers working with older Objective-C codebases or interacting with non-ARC libraries. 

**Understanding the Issue:**
In Objective-C's manual reference counting, objects must be retained when they're in use and released when they're no longer needed. Failing to maintain a proper balance between retains and releases can lead to crashes.

**How to Run:**
1. Clone this repository.
2. Open the project in Xcode.
3. Run `bug.m` to observe the crash.
4. Modify the code to match `bugSolution.m` to see the corrected implementation.

**Keywords:** Objective-C, Memory Management, retain, release, ARC, EXC_BAD_ACCESS, Crash, Segmentation Fault