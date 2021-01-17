# youtube-dl-cheatsheet


## Installing youtube-dl
Install youtube-dl using pip:
```
pip install --upgrade youtube-dl
```
Install youtube-dl using Homebrew:
```
brew install youtube-dl
```

## youtube-dl general command format
```
youtube-dl [OPTIONS] URL [URL...]
```

## Downloading videos
To download Youtube videos use the following commands and replace URL with a valid Youtube video URL

 **Download video using default options**
Used when you want to download the best available quality without specifying any extra options
```
$ youtube-dl URL
```
**Retrieve all available formats**
```
$ youtube-dl -F URL
```
after using this command, you can proceed to download a video in a specific format using the format code. For example let's assume the format you want to download has the format code 135, you can download it using the following command:
```
$ youtube-dl -f 135 URL
```
**Limit download speed**
You can specify maximum download speed in bytes like this:
```
$ youtube-dl -r 10240 URL    # Download speed is limited to 10240 bytes (10 KB)
```
or in KB:
```
$ youtube-dl -r 10K URL    #Download speed is limited to 10KB
```
or in MB:
```
$ youtube-dl -r 10M URL    #Download speed is limited to 10MB
```
