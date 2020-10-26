## Turn ptr2besms edits into .iso edits

[← Home](https://ptrguide.github.io)

### Steps:

0. Open your custom lines using ptr2besms.

1. Open the stage you edited and pause on it.

2. Open Cheat Engine's Memory Viewer and the stage's OLM (in a hex editor).

3. In the OLM, start selecting around 2-3 lines of bytes near the start but NOT AT THE START.  (Stage 1 good point starts at 00001100)

4. In Cheat Engine, search for an array of bytes and paste your hex in.

5. If needed, scroll up to the point where your hex starts to match with the OLM.

6. now its time for some M A T H 

go to this quality site, itll help - [http://www.calculator.net/hex-calculator.html](http://www.calculator.net/hex-calculator.html)

do the following:

END ADDRESS OF OLM - ADDRESS OF YOUR OLM GOOD POINT

----get the hex output, then do the following

START ADDRESS OF GOOD SPOT IN CHEAT ENGINE + HEX OUTPUT FROM BEFORE

----that will be your endpoint.

7. Inject your custom lines.

8. In Cheat Engine's Memory Viewer (which you should already have open from step 2), goto File > Save Memory Region.

Un-check the header box and input your start and end values.

Save it to a place where you can remember.

9.  Open your CEM in a hex editor.

Select all of it, hit CTRL+C, then go to your OLM hex and CTRL+B it into the good point.

10. Save your OLM, compile the iso, and there you go!
