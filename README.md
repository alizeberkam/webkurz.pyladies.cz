# webkurz.pyladies.cz

This is more or less temporary website based on older materials from different sources. That's why it's software architecture is a bit weird.


## Install

With node.js installed run

```shell
sudo npm i gulp-cli -g
```

```shell
npm i
```


## Development

Enjoy automatic refreshing of everything by running.

```shell
gulp develop
```

The website will run on [http://localhost:3030](http://localhost:3030).


## Content writing

Add .md files in subfolders of `/lekce/`. Required HTML files are created automatically.

Don't forget to add/remove links to files to `/_menu.html` and to `/index.html`. 


### Inside .md

Top sections are divided by `\n---\n` while subsections are divided by `\n----\n`.
 
For tasks add `<!-- .slide: data-state="c-slide-task" -->` at the beggining of the section.

Put HTML examples into `<div class="c-example example-foo">` where `example-foo` is a name of your choice and add styling to `examples.scss` file.



## Deployment

With installed surge client (`npm i surge -g`) run

```shell
gulp deploy
```

Note: you need to have access to surge account (just ask Dan Srb).


