### Install

[reference](https://github.com/shawncplus/phpcomplete.vim/wiki/Getting-better-tags)

#### step

    wget "https://github.com/shawncplus/phpcomplete.vim/raw/master/misc/ctags-5.8_better_php_parser.tar.gz" -O ctags-5.8_better_php_parser.tar.gz
    tar xvf ctags-5.8_better_php_parser.tar.gz
    cd ctags

    autoreconf -fi
    ./configure
    make

    sudo make install

#### use

    cd /path/to/your/projects/root
    ctags -R --fields=+laimS --languages=php src
    ctags -R --fields=+laimS --languages=php -f tags.vendors vendor
