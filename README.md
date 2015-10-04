# ec2-ssh
Scripts to ssh to ec2 instances by tag or name with tmuxinator

## Installation:
* Install tmux
* Install [tmuxinator](https://github.com/tmuxinator/tmuxinator)
* ```
git clone git@github.com:orimarti/ec2-ssh.git
chmod +x ec2-ssh/*
echo "export PATH=$PATH:`pwd`/ec2-ssh/" >> ~/.bashrc
```
## Usage:
```
ec2-ssh instance_name
ec2-ssh <tag_name> <tag_value>
```
If only one instance it's found it will access directly through 
ssh, if more than one instance is found it will create a 
[tmuxinator](https://github.com/tmuxinator/tmuxinator) template and 
access through it
