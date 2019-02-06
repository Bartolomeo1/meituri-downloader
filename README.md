# Meituri Album Downloader

**Not safe for work (NSFW)**.  
A command line script that lets you download albums with given IDs from meituri.com. You need the album ID and the number of photos in an album to start downloading the images.

## How to

Usage in command line:

`meituri.py album_id num_of_pics`

### Example:
`meituri_downloader.py 14449 55`

![](screenshot_site.png)

![](screenshot_cmd.png)
### Explanation:
Attempts to download the album with the ID of 14449 that has 55 pictures in it.  
URL of the example: https://www.meituri.com/a/14449/

IDs are in the URL when viewing an album after the /a/ and before whatever page you might be on.  
Same example with page:	https://www.meituri.com/a/14449/2.html  
ID is 14449.

Number of pictures are located on top of the page with the other set info.
```
  拍摄机构： [agency name]
  图片数量： 55P <-- Number of pictures, has a P next to it
  发行日期： 2016-03-04
```
Model name and info is below the information above on the website if you want to check more of the model.
