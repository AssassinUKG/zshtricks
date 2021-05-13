# zshtricks

### NotifyJobs

## Setup

Edit .zshrc file, add the below code to the end

```zsh
function notifyJob(){
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
# command ; notifyJob Name

nmap -v 192.168.1.1 ; notifyJob nmap
```

## Screenshot

![](Capture.PNG)
