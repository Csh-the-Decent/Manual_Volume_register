
**This matlabapp is written to maunally register each Z plane in each volume.**

## Workflow
1. Load a Stack. File>Load
2. In "View" mode, Select a Z plane as fixed.(Soma suggested)
3. Change to "Register" mode, Compare the nearest 2 planes and move one of them to register.
4. "Z project" mode, Preview the result.
4. File>Save
4. File>Close
4. the next stack


## Codes Consist of 
- loading
    - load an ims file
    - get its properties
    - ensure it contains one volume and get its Z plane number and x&y pixel number
    - convert it into xyz 3-dim matrix
- Image Window
    - Show two nearing image at the same time (with Different Color)
    - Alpha (Transparent)
- Z projection
    - a button to z-project the current stack
- Change the current Z plane
    - up/down 1 plane (next)
    - number(jump to)
    - Select as the fixed  plane
- Move image
    - an x slider
    - an y slider
    - an angle knob

- Other commands
  - Save as
  - Close the current stack