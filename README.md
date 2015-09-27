blogger2md
==========

Given a Blogger export in xml atom format, `blogger2md` exports the source XML for each blog post, then converts each blog post into a markdown file (`.md`), and an HTML file.

## Usage
    python blogger2md.py --output-dir your/directory/ blogger_file.xml

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

### "Content Unavailable" Errors

If the HTML files contain the string "Content Unavailable", it means that `blogger2md` was unable to retrieve the content from an HTTP request to the specified post. Check the URL of the content in the corresponding XML file. The URL will be in a `<link>` element with the `rel` attribute of 'alternate'. Visit this URL in the browser, and it should be clear why the content is unavailable!

## Credits
This code is based on a [script by @larsks](https://gist.github.com/larsks/4022537).
