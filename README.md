# Bash alias
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

you need to check the folders in the cd file, they are specifically set for me

you can replace some with the following command:
```
sed -i 's-/Users/bart/dev-/Users/user_dir-' cd
```
