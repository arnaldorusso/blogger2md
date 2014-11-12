blogger2md
==========

Given a Blogger export in xml atom format, `blogger2md` converts each
blog post into markdown. A `.md` file is created for each post.

## Usage
    python blogger2md.py --output-dir your/directory/ --html2text blogger_file.xml

### Help

~~~ sh
$ python blogger2md.py --help
usage: blogger2md.py [-h] [--online] [--pandoc] [--html2text]
                     [--output-dir OUTPUT_DIR]
                     input

positional arguments:
  input

optional arguments:
  -h, --help            show this help message and exit
  --online, --fuckyeah
  --pandoc
  --html2text
  --output-dir OUTPUT_DIR, -d OUTPUT_DIR
~~~

## Credits
This code is based on a [script by @larsks](https://gist.github.com/larsks/4022537).
