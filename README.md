# Reddit2Wallpaper
Very (very) simple Golang app that downloads photos from Reddit's `r/EarthPorn` subreddit
and saves them in a directory of choice.  
It can also filter out photos with less than the specified resolution.

Note: it will probably work with other subreddits (just use the `-subreddit` command line
argument), but it won't filter by resolution unless the post has `<width>x<height>` somewhere
in the title, like on `r/EarthPorn` and `r/wallpapers`.

## Usage
```
Usage of reddit2wallpaper:
  -download_dir string
        Directory in which to save wallpapers
  -minheight int
        Minimum height for the photo to download
  -minwidth int
        Minimum width for the photo to download
  -ratio_height int
        Aspect ratio height
  -ratio_width int
        Aspect ratio width
  -subreddit string
        Name of the subreddit to use (default "EarthPorn")
  -top_posts
        Fetch 'top' posts instead of 'new' posts
```

## How to install
If you have Go already installed you can run the following in your command line:
```
go install github.com/mattiamari/reddit2wallpaper/cmd/reddit2wallpaper
```

To update, just run the command above again.

You can also download a [precompiled binary](https://github.com/mattiamari/reddit2wallpaper/releases).

I tested the Linux and Windows ones but not the one for OSX, so if that doesn't work just let me know :)
