# Detect Blur

When run, detectBlur.sh iterates through a directory of images and allows the user to act on those that are more blurry then a defined value (set using the 'definedThreshold' variable (the default being 0.004 -- 0.4%)).

detectBlur.sh can be run periodically as a cron job by editing your users crontab file

```
crontab -e
```

and adding a new job for the script

```
* * * * * /path/to/detectBlur.sh
```

The above will, for example, run the script once every minute.

This script depends on 'ImageMagick' and 'bc'. Both of which are installed by default on most Linux distributions.
