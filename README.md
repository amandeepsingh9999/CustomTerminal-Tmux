# CustomTerminal-Tmux

[![Watch the video](https://img.youtube.com/vi/7poUgkPtEA8/hqdefault.jpg)](https://www.youtube.com/watch?v=7poUgkPtEA8)

# Tmux -
A terminal multiplexer lets you use the terminal as in tile format
and also creates session that can be changed with prefix and n,p
n in stand for next , p stand for previous 

## Installation 
#### Ubuntu - 
###### Make sure the repositories are up to date and then install tmux
```
sudo apt update
sudo apt install tmux
```
#### MacOs -
###### step -1 If you don't have home brew installd then install it using
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
###### Step - 2 Install tmux 
```
brew install tmux

```
### Tmux Package Manager
we willbe using this package manager for our further process 

#### Requirements 
`Tmux` `git` `bash` or make sure you have this according to your os

#### Clone TPM
```
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
#### Dot-file
we have to create this file using touch or what ever you like 
```
touch ~/.tmux.conf

OR

touch $XDG_CONFIG_HOME/tmux/tmux.conf
```
All of our configuration will sit here\
let's put a example config 
```
set -g mouse on
```
save it and get back to tmux terminal and run 
```
tmux source ~/.config/tmux/tmux.conf
```

## Prefix key 
All of the tmux shortcuts will use this key which is `ctrl + b` , we will be changing it to some other key we will use whatever suits us comfortable

## Splitting the term
These pains are tiled perfectly and also you can adjust their sizes as you like with 
```
ctrl + b Arrow 
```
> NOTE you need to keep pressing the prefix key until you get size of your comfort
#### Horizontal split
```
ctrl + b "
```
#### Vertical Split
```
ctrl + b % 
```

> Note: Please use shift key for `"` & `%`


## Setting up config
### TPM 
Put this in on your `tmux.conf`
```
set -g @plugin 'tmux-plugins/tpm'
set -g @plugin 'tmux-plugins/tmux-sensible'

run '~/.tmux/plugins/tpm/tpm'
```
> NOTE: This should be in the bottom of your `tmux.conf` file

Then do the step below to install the `TPM` in your tmux
```
ctrl + b + Shift + i
```
