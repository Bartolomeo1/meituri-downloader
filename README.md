# :ribbon: Meituri Album Downloader

**Not safe for work (NSFW)**.  
A command line script that lets you download albums with given IDs from [meituri.com](https://www.meituri.com/).  
The album ID and the number of photos in the album are needed inputs to start downloading the images.


Requires `click` to work with CLI arguments.  
```
Usage: meituri.py [OPTIONS]

Options:
  -a, --album INTEGER   Album ID located in the URL:
                        https://www.meituri.com/a/$ID
  -n, --number INTEGER  Number of pictures on top of the page followed by P.
  -h, --help            Show this message and exit.
```

**(12th of March of 2019) Notice:** After adding a minimum of 5 seconds time delay between downloads, they seem to work fine.

**(24th February of 2019) Notice:** I'm getting `an existing connection was forcibly closed by the remote host` error or it just hangs still (can't even CTRL + C) after 5-6 images. Maybe it's just me.

## How to

First install `click` by running the following:

```
pip install -r requirements.txt
```

Usage in command line:

```
python meituri.py -a album_id -n num_of_pics
```

### Example:
`python meituri.py -a 14449 -n 55`

![](extras/screenshot_site.png)

### Explanation:
Attempts to download the album with the ID of 14449 that has 55 pictures in it.  
URL of the example: https://www.meituri.com/a/14449/

IDs are in the URL when viewing an album after the `/a/` and before whatever page you might be on.  
Same example with page:	https://www.meituri.com/a/14449/2.html  
ID is 14449.

Number of pictures are located on top of the page with the other set info.
```
  拍摄机构： [agency name]
  图片数量： 55P <-- Number of pictures, has a P next to it
  发行日期： 2016-03-04
```
Model name, alias and other info is below this information on the website if you want to check more of the model.

### Result:

_On a different gallery but still_.

![](extras/screenshot_urxvt.png)
