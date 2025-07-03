# Bash aliases
These are some aliases / functions that I use to make my life easier, you might find some useful, some not so much

## Getting started
I recommend placing the scripts in your code / scripts folder, not directly in ~,
Just make a symlink, you can do this per person or in root
```bash
cd ~/scripts
git clone git@github.com:bnoordsij/bash-aliases.git

# asuming you want to set it for root as well
sudo su

# symlink
ln -s ~/code/scripts/bash-aliases ~/bash-alias

# add aliases in startup script
vi +999 ~/.bashrc
# vi +999 ~/.profile # for mac
```

add the following in `.profile` or `.bashrc`
```
source ~/bash-alias/main
```


## cd
there used to be a file called cd, it contained specific aliases for cd'ing to certain folders, but only for my Mac
you can add your own cd file, if it exists it will be loaded.

These were some aliases that were in there to give you an idea:
```bash
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

some things you can put in there:
```bash
# prevent accidental rm, can be overruled with rm -f
#alias rm='rm -i'
```
