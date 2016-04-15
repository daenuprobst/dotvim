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

Thanks
------
Artem Dudarev
