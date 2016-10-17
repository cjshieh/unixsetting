# unixsetting
unix setting for mac os

$brew install zsh

install oh my zsh

$sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

https://github.com/robbyrussell/oh-my-zsh


$brew install tmux

$brew install ctags

$brew install luajit

$brew install chruby

$brew install mercurial


LINUX

sudo apt-get update

sudo apt-get install git-all

sudo apt-get install tmux

installing zsh 

sudo apt-get install zsh

curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sudo sh

can skip this… if point 2 is done correctly.

sudo chsh -s /bin/zsh

or 
sudo vim /etc/passwd
change the last line


chmod +x install_vim_lua.sh

./install_vim_lua.sh

Set up Vundle:

$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

https://github.com/VundleVim/Vundle.vim


Install Plugins:

Launch vim and run :PluginInstall

To install from command line: vim +PluginInstall +qall

Place onedark.vim in your ~/.vim/colors/

mkdir ~/.vim/colors

mv onedark.vim ~/.vim/colors

reference from

http://rick.cogley.info/post/use-homebrew-zsh-instead-of-the-osx-default/
https://github.com/robbyrussell/oh-my-zsh/wiki/Plugin:git
https://github.com/bobthecow/git-flow-completion
https://github.com/elsdrm/.unix_settings





Some bugs related to AWS EC2 

http://blog.leanote.com/post/hugo/complete-13-command-not-found-compdef

change the shell in tmux to zsh

$chsh -s $(`which zsh`) $USER



install latest version tmux

sudo yum install libevent-devel 

	$ git clone https://github.com/tmux/tmux.git
	$ cd tmux
	$ sh autogen.sh
	$ ./configure && make


build vim from source with lua

git clone https://github.com/vim/vim

cd vim/src

sudo make distclean

sudo ./configure --with-features=huge \
            --enable-rubyinterp \
            --enable-largefile \
            --disable-netbeans \
            --enable-pythoninterp \
            --with-python-config-dir=/usr/lib/python2.7/config \
            --enable-perlinterp \
	    --enable-luainterp=dynamic \
	    --enable-gui=auto \
            --enable-fail-if-missing \
            --enable-cscope \
            --enable-multibyte \
    	    --enable-gpm \
    	    --enable-cscope \
	    --enable-fontset

sudo make 

sudo make install

