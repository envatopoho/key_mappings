## Git Tab Completion

http://code-worrier.com/blog/autocomplete-git/

First get the `git-completion.bash` script and put it in your home directory:

```
curl https://raw.githubusercontent.com/envatopoho/key_mappings/master/dotfiles/.git-completion.bash -o ~/.git-completion.bash
```

And then add this to your `.profile`(osx)  or `.bash_profile`(linux)
```
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```
