# Online class auto join and greet
macOS Automator script that can be triggered by a calendar event’s alert. It will automatically open the class URL, log in (if needed), join the class and send a custom greeting message in the chat-box. Compatible with famous Iranian meeting service “Skyroom.”

## Initial setup
1. Download, extract and open `guest-greeting.workflow.zip` for guest classes and `user-greeting.workflow.zip` for classes that need user authentication.
2. Replace `https://www.example.com` on the first task with your URL.
3. In the shell script box `cat /Users/examplePath/greeting.rtf | pbcopy` replace the example path with your greeting rich-text-format file path. (Using plain text file `.txt` may prevent the text from getting pasted.)


### Join class as a user
4. In the shell script box `cat /Users/examplePath/username.txt | pbcopy` (and the other one for the password), replace the example path with your username and password plain text file path. (Using rich-text-format file file `.rtf` may prevent the text from getting pasted.)

## Triggering by macOS Calendar event
1. Convert your workflow to an application. (`⌥⇧⌘C`)
2. Add an alert for your event and set the custom alert to open the automation file.
