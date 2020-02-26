# PHP Extension Development Tutorial

Environment:

Mac Os X 10.14.4

## 1.Clone PHP Source First

```
https://github.com/php/php-src.git
```

### git checkout php-xx.xx.xx whatever you want that version you build



## 2.Build PHP Source

```
./configure
```

## 3.Create A new extension with ext\_skel

```
➜  php-src git:(php-7.2.9) ✗ cd ext
➜  ext git:(php-7.2.9) ✗ ./ext_skel --extname=test1


Creating directory test1
Creating basic files: config.m4 config.w32 .gitignore test1.c php_test1.h CREDITS EXPERIMENTAL tests/001.phpt test1.php [done].

To use your new extension, you will have to execute the following steps:

1.  $ cd ..
2.  $ vi ext/test1/config.m4
3.  $ ./buildconf
4.  $ ./configure --[with|enable]-test1
5.  $ make
6.  $ ./sapi/cli/php -f ext/test1/test1.php
7.  $ vi ext/test1/test1.c
8.  $ make

Repeat steps 3-6 until you are satisfied with ext/test1/config.m4 and
step 6 confirms that your module is compiled into PHP. Then, start writing
code and repeat the last two steps as often as necessary.
```



