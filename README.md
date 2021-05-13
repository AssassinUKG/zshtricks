# zshtricks

### NotifyJobs

## Setup

Edit .zshrc file, add the below code to the end

```zsh
function runNotifyJob(){
notify-send -u critical -i "notification-message-IM" "Job Finished" "Job Completed: $1"
}

```
Then source the .zshrc file
```zsh
. ./.zshrc
```

## Usage 

Use the command to run a long running task and send a notification to the desktop

```zsh
# command ; runNotifyJob Name

nmap -v 192.168.1.1 ; runNotifyJob nmap
```

## Screenshot

![](Capture.PNG)
