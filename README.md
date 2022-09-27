# neorg-ascii
**This project is not complete, not even started, I'm only capturing some ideas for reference and to allow other people to give ideas**


# Neorg Bookmark Manager
**This project is not complete, not even started, I'm only capturing some ideas for reference and to allow other people to give ideas**

This module for [Neorg](https://github.com/nvim-neorg/neorg) is to insert ASCII text and possibly art into a norg file.

## Features
**Still a work in progress, these are only planned features**

### Create ASCII text
`= ASCII ONLY@ neorg`

Would produce
```
@    @  @@@@@@  @@@@   @@@@@    @@@@
@@   @  @      @    @  @    @  @    @
@ @  @  @@@@@  @    @  @    @  @
@  @ @  @      @    @  @@@@@   @  @@@
@   @@  @      @    @  @   @   @    @
@    @  @@@@@@  @@@@   @    @   @@@@
```

### Create ASCII art
`= ASCII ART open_book`

Would produce
```
      ______ ______
    _/      Y      \_
   // ~~ ~~ | ~~ ~  \\
  // ~ ~ ~~ | ~~~ ~~ \\
 //________.|.________\\
`----------`-'----------'
```
### Let people define ASCII font files
Not sure how to implement that yet, initial thought is to simply define a `ascii-font` directory inside a workspace with neorg files as font files.

For example:
inside `workspace/ascii-font/only@.norg`
```
#contexts A
   @
  @ @
 @   @
@     @
@@@@@@@
@     @
@     @

#contexts B
@@@@@@
@     @
@     @
@@@@@@
@     @
@     @
@@@@@@
```
all the way from A-Za-z0-9 etc
