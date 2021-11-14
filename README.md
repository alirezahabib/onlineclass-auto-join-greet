# Online class auto-join and greet
macOS Automator script that a calendar event’s alert can trigger. It will automatically open the class URL, log in (if needed), join the class and send a custom greeting message in the chatbox. Compatible with famous Iranian meeting service “Skyroom.”

## Initial setup
1. Download, extract and open `guest-greeting.workflow.zip` for guest classes and `user-greeting.workflow.zip` for rooms that need user authentication.
2. Replace `https://www.example.com` on the first task with your URL.
3. In the shell script box `cat /Users/examplePath/greeting.rtf | pbcopy`, replace the example path with your greeting rich-text-format file. (Using plain text file `.txt` may prevent the text from getting pasted.)


### Join the class as a user
In the shell script box `cat /Users/examplePath/username.txt | pbcopy` (and the other one for the password), replace the example path with your username and password plain text file. (Using rich-text-format file `.rtf` may prevent the text from getting pasted.)

4. Run and test the workflow. You may rerecord the corresponding “Watch Me Do” section(s) if something goes wrong.

## Triggering by macOS Calendar event
1. Convert your workflow to an application. (`⌥⇧⌘C`)
2. Add an alert for your event and set the custom alert to open the automation file.
3. You may need to grant some permissions the first time.
