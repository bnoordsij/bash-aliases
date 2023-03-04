# Bash aliases
These are some aliases / functions that I use to make my life easier, you might find some useful, some not so much

## Getting started

```
cd ~
git clone git@github.com:bnoordsij/bash-aliases.git bash-aliases
```

in .profile or .bashrc
`source ~/bash-aliases/main`

### alternative place
you can clone the repo in a different place, let's say ~/code/scripts/bash-aliases
in that case you must make a symlink to the folder, otherwise the relations won't work
```
ln -s ~/code/scripts/bash-aliases ~/bash-aliases
```

## cd
there used to be a file called cd, it contained specific aliases for cd'ing to certain folders, but only for my Mac
you can add your own cd file, if it exists it will be loaded.

These were some aliases that were in there to give you an idea:
```
## absolute
alias cddown='cd /Users/bart/Downloads/; '
alias cddev='cd /Users/bart/dev/; '
alias cdtu='cd /Users/bart/dev/klanten/werkenbijtechnischeunie.nl; '

## relative
alias cdrmod='cd ./vendor/laravel-modules; '
alias cdrcore='cd ./vendor/laravel-modules/core; '
```

## local
If you have your own bash_aliases it is recommended to put them in the local file

this will keep it organized

it is the last script that is run, so every command should be available to you
