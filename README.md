# Chrome-Terminal-Script-to-Copy-Slack-Message-Text
If you are looking at Slack in Chrome and open up developer tools, you can go to the terminal part of developer tools and paste this. It will scroll up and copy text for 5 minutes, or for this week, or for messages from today, then download to your computer.


Slack Channel Text Export (Chrome DevTools Method)

This guide explains how to export Slack channel messages as plain text using Chrome Developer Tools.

Requirements

Google Chrome

Access to the Slack channel in a browser

The export script provided separately

Step 1: Open Slack in Chrome

Open Google Chrome.

Go to your Slack workspace (for example: https://app.slack.com
).

Navigate to the channel you want to export.

Click inside the message list once to ensure it has focus.

Step 2: Open Developer Tools

You can open Chrome Developer Tools in any of these ways:

Press F12

Press Ctrl + Shift + I (Windows)

Press Cmd + Option + I (Mac)

Right click anywhere on the page and click Inspect

Step 3: Open the Console Tab

In Developer Tools, click the Console tab.

Click inside the console input area so the cursor is active.

If Chrome blocks pasting:

Type allow pasting

Press Enter

Then paste your script again

Step 4: Run the Script

Paste the Slack export script into the Console.

Press Enter.

The script will begin scrolling and collecting messages.

You will see progress logs appear in the Console.

Step 5: Stop the Script (Optional)

To stop early and download immediately:

stop()


Or:

slackDump.stop()


When the script finishes or is stopped, a .txt file will automatically download.

Output

The downloaded file contains:

Username: message text


Images and GIFs are not included.

Messages are filtered by the script’s configured date range (for example, today or this week).

If Nothing Scrolls

Click inside the message list area and run the script again.

Make sure you are in a Slack channel view, not a thread panel or DM popout.
