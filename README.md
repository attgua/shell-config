# shell-config


Open the terminal and set::

```
vim ~/.zshrc
```


```
autoload -Uz compinit
compinit

source <(kubectl completion zsh)

alias k=kubectl
complete -F __start_kubectl k
zstyle ':completion:*' menu select=2 
```


Activate the settings:

``` 
source ~/.zshrc
```