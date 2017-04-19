Add the following to your `~/.profile` to: 

**Have tab completion of git repos (copy the `.git-completion.bash` file first):**
```
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```

**Have tab completion of aws-vault commands**
```
complete -o "default" -o "nospace" -W "$(sed -E -e '/^\[profile.*/!d' -e 's/^\[profile (.+)\]/\1/g' ~/.aws/config)" aws-vault;
```
