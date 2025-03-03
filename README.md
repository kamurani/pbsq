# pbsq


## Installation 

`pip install pbsq` 

## VScode

To use the `launch` command, you will need to have `VS code` added to your `$PATH`. 
#### Using command palette 

In VS code, open the **command palette** (`Cmd+Shift+P`), type "shell command",
and run the `Shell Command: Install 'code' command in PATH` command.
#### Manually configure the path 

##### Zsh 

```zsh
cat << EOF >> ~/.zprofile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"
EOF
```
##### Bash
```bash
cat << EOF >> ~/.bash_profile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"
EOF
```
Restart your shell to register your changes.  You can check with `which code`.
### Enable tab completion for Bash, Fish, or Zsh


> After modifying `.rc` files for your shell, you may have to restart the shell to enable completions. 
#### Zsh

```zsh
_PBSQ_COMPLETE=zsh_source pbsq > ~/.zsh/pbsq-complete.zsh
```
> NOTE: you may have to add `source ` to your `~/.zshrc` if this does not work.  
#### Bash 
```bash
_PBSQ_COMPLETE=bash_source pbsq > ~/.pbsq-complete.bash
```
Add the following to your `~/.bashrc`:
```bash
. ~/.pbsq-complete.bash
```
#### Fish 
```fish
_PBSQ_COMPLETE=fish_source pbsq > ~/.config/fish/completions/pbsq.fish
```
