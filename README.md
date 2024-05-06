# Image Compression Script

A command line script that compresses image(s) as much as possible with minimal loss to quality or resolution.
The script supports JPEG, PNG and WEBP image formats and is built using open-source modules.

## Requirements
- Python 3.x
- PIL (Pillow)

## Installation
To use this script, ensure you have Python installed on your system. If not, you can download it from [python.org](https://www.python.org/downloads/). You will also need the `dnspython` library, which can be installed via pip. Here’s how to set up your environment:

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```


## Usage
`python CompressImage.py -f [file or directory path] -q [quality]`
- `-f` or `--file`: path of the image file or directory containing the images.
- `-q` or `--quality`: quality of compression from 0 to 100 (default is 95).
- `-h`: show help 

## Example
```shell
python CompressImage.py -f test/TestImage-Canon_40D.jpg -q 85
```

or

```shell
python CompressImage.py -f test -q 75
```

## Notes
Currently the script only works for jpeg, png and webp files and you can extend it to other image file formats as well.
