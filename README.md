# conn-jenkins-to-gh-LI-jbenj
Creating the README after the repo was created
WebHooks has been added by 
### clicking 'Copy link address' on the pipeline's main page
### selecting 'Settings' and 'WebHooks' in GitHub and clicking 'Add WebHook'
### adding the copied link address and adding 'github-webhooks/' to the end of it

Adding a change to push and trigger a build.
Trying again at 1:08 PM est.
Trouble shooting 'ECONNREFUSED'.
Updated port from 8080 to 80, per this output in the terminal:
![image](https://github.com/jbenj-upenn/conn-jenkins-to-gh-LI-jbenj/assets/59940368/a589d508-744c-45e5-9d39-92484267d818)

Searched 'smee.io ECONNREFUSED TCPConnectWrap.afterConnect'
Changed port of smee to 8089 with the command:  smee --url https://smee.io/3vcoqlVpo6Bxldci --path /github-webhook/ --port 8099
Back to port 8080

New Webhook set up and connected with command: >smee --url https://smee.io/sIqX3xPeRfNfZGQ --path /github-webhook/ --port 8080
