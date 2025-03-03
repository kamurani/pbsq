# pbsq


## Installation 

`pip install pbsq` 

## Shell completions 

> After modifying `.rc` files for your shell, you may have to restart the shell to enable completions. 
### ZSH

```zsh
_PBSQ_COMPLETE=zsh_source pbsq > ~/.zsh/pbsq-complete.zsh
```
> NOTE: you may have to add `source ` to your `~/.zshrc` if this does not work.  
### Bash 
```bash
_PBSQ_COMPLETE=bash_source pbsq > ~/.pbsq-complete.bash
```
Add the following to your `~/.bashrc`:
```bash
. ~/.pbsq-complete.bash
```
### Fish 
```fish
_PBSQ_COMPLETE=fish_source pbsq > ~/.config/fish/completions/pbsq.fish
```
