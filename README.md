# TTYGIF

> ttygif converts a ttyrec file into gif files.
> It's a stripped down version of ttyplay that captures every frame.

## Note

On my mac ( El Capitan ), I still got an error :
9:31: execution error: Can’t get application "Apple_Terminal". (-1728)
After a little googling I found out it is because of env variable $TERM_PROGRAM so I made a little change and now it is working like a charm.

## Setup

### OSX
``` sh
$ brew install https://raw.githubusercontent.com/icholy/ttygif/master/ttygif.rb
```

## Usage:

**1. Create ttyrec recording**

``` sh
$ ttyrec myrecording
```

* Hit CTRL-D or type `exit` when done recording.

**2. Convert to gif**

``` sh
$ ttygif myrecording
```

On OSX optionally you can set a -f flag which will bypass cropping which is needed for terminal apps which aren't full screen. 
Both standard Terminal and iTerm apps are supported.

``` sh
$ ttygif myrecording -f
```

## Demo:

![gif](http://i.imgur.com/nvEHTgn.gif)

## Credits

The idea and approach was adapted from [tty2gif](https://bitbucket.org/antocuni/tty2gif)

![](http://i.imgur.com/9et8daN.jpg)

