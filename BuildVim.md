# How to build vim from source

## Get source code
`git clone https://github.com/vim/vim.git`

## Install dependencies

```
ncurses-devel
ruby-devel
python-devel
lua-devel
perl-ExtUtils-Embed
```

## configure
```
./configure \
        --enable-multibyte \
        --with-features=huge \
        --enable-luainterp \
        --enable-perlinterp \
        --enable-pythoninterp \
        --with-python-config-dir=/usr/lib64/python2.7/config \
        --enable-rubyinterp \
        --with-ruby-command=/usr/bin/ruby \
        --enable-fail-if-missing
```

## make

`make`

If there is no error, check if the option is valid.

`./src/vim --version`

## install

`make install`

