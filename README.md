Vim Configuration
=================
This is my humble vim configuration (dotfile).

Getting it up and running
-------------------------

```
git clone https://github.com/daenuprobst/dotvim.git ~/.vim
ln -s ~/.vim/vimrc ~/.vimrc
cd ~/.vim
git submodule init
git submodule update
```

Installing a plugin (submodule)
-------------------------------
Installing, for example, the fugitive (git wrapper) plugin:

```
cd ~/.vim
git submodule add http://github.com/tpope/vim-fugitive.git bundle/fugitive
git add .
git commit -m "Added the fugitive plugin."
```

Upgrade the plugins
-------------------
To upgrade all the plugins in the bundles folder:

```
cd ~/.vim
git submodule foreach git pull origin master
```

YouCompleteMe
-------------
In order to get the autocomplete working, do the following:

```
cd ~/.vim/bundles/youcompleteme
git submodule update --init --recursive
./install.sh --clang-completer --tern-completer (clang for c-like support requires clang, tern for js support requires nodejs and npm)
```

Thanks
------
Artem Dudarev
vimcasts.org
