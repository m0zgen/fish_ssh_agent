# fish_ssh_agent

![Custom badge](https://img.shields.io/endpoint.svg?cacheSeconds=1&logo=gitlab&label=gitlab&message=HELLO&style=popout&url=https%3A%2F%2Fgitlab.com%2Fkyb%2Ffish_ssh_agent%2Fraw%2Ftemp-badge%2Fbadge-gitlab.json)
![Custom badge](https://img.shields.io/endpoint.svg?cacheSeconds=1&logo=github&style=popout&url=https%3A%2F%2Fgitlab.com%2Fkyb%2Ffish_ssh_agent%2Fraw%2Ftemp-badge%2Fbadge-github.json)

Utility functions to start your ssh agent when using fish shell.
You will only need to run `ssh-add` and type your password once,
after the running ssh_agent should do the work for you.


## Usage

```fish
fish_ssh_agent
```


## Installation

```fish
wget https://gitlab.com/kyb/fish_ssh_agent/raw/master/functions/fish_ssh_agent.fish -P ~/.config/fish/functions/
```

### Autostart
Append next line to `~/.config/fish/config.fish`
```fish
fish_ssh_agent
```


## Useful note
Add this line to `~/.ssh/config`
```
AddKeysToAgent yes
```
With option enabled keys used by ssh will be automatically added to ssh-agent. No need to call `ssh-add`.


## Mirrors
https://gitlab.com/kyb/fish_ssh_agent  
https://github.com/ivakyb/fish_ssh_agent  
