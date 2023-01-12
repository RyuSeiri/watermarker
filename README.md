# marker.py

为图片添加文字水印的一个Python脚本
可设置文字**大小、颜色、旋转、间隔、透明度**

# usage

- 运行脚本前的操作，首先需要安装Pillow：  
 `pip install Pillow`

- 运行脚本的命令如下：  
`python marker.py -f ./input/test.png -m Watermarker`

- 更多详细请参照下面： 
```
usage: marker.py [-h] [-f FILE] [-m MARK] [-o OUT] [-c COLOR] [-s SPACE] [-a ANGLE] [--font-family FONT_FAMILY] [--font-height-crop FONT_HEIGHT_CROP] [--size SIZE]
                 [--opacity OPACITY] [--quality QUALITY]

optional arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  image file path or directory
  -m MARK, --mark MARK  watermark content
  -o OUT, --out OUT     image output directory, default is ./output
  -c COLOR, --color COLOR
                        text color like '#000000', default is #8B8B1B
  -s SPACE, --space SPACE
                        space between watermarks, default is 75
  -a ANGLE, --angle ANGLE
                        rotate angle of watermarks, default is 30
  --font-family FONT_FAMILY
                        font family of text,using font in system just by font file name
                        for example 'PingFang.ttc', which is default installed on macOS
  --font-height-crop FONT_HEIGHT_CROP
                        change watermark font height crop
                        float will be parsed to factor; int will be parsed to value
                        default is '1.2', meaning 1.2 times font size
                        this useful with CJK font, because line height may be higher than size
  --size SIZE           font size of text, default is 50
  --opacity OPACITY     opacity of watermarks, default is 0.15
  --quality QUALITY     quality of output images, default is 90
```






