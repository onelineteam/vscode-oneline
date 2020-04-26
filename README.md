# oneline README

oneline is a plugin to increase development speed. you can use the commands in the current file.

the website: [http://www.onelineteam.com](http://www.onelineteam.com)

## Features

all commands currently only support the relative path.

## usage

type command line and select it.

- tap shortcut for the command palette, exec command:  `oneline`.

- or tap (mac: `cmd + r`, window: `ctrl+alt+r`) shortcut for running `oneline`.

**demo:**

![demo](https://github.com/onelineteam/vscode-oneline/blob/master/assets/images/oneline-rp.gif?raw=true)

if you want to join us, please scan the image below to be friend with me by wechat's scan.

![bboyer](https://github.com/onelineteam/vscode-oneline/blob/master/assets/images/bboyer.jpeg?raw=true)

or you can follow the wechat public account. 

![onelineteam](https://github.com/onelineteam/vscode-oneline/blob/master/assets/images/oneline-wechat-public-qr.jpg?raw=true)


## cp

copy file content to the target file.

```shell
  cp [source] -o [target]|[here]
```

"source" is source file.

`-o` set the target file. it have a optional value is **here**. **"here"** means the current cursor position.

### find

search file and show the results.

```shell
  find [name] -d [dir] -R
```

"name" is your search key. it's required.

`-d` the search directory. it's required.

`-R` recursive search.

### from

write some content to the target file.

```shell
  from `[content]` -o [target] -p [position]
```

`-p` position's format like "row:col". if col's value is end, the col's position is length of the current line.

`-o` target file. it's a relative path of the current file. it's required.

### to

jump to the target file.

```shell
  to [target]
```

"target" is required.

### rp

replace text. support regex.

```shell
  rp source target
  #or
  rp `source/target,source/target........`
```
