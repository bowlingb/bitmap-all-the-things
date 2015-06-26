# B.A.T.T. - Bitmap All The Things

## Description

B.A.T.T. converts bits into bitmaps, and bitmaps back into bits. 

By default, B.A.T.T. enc any given file or directory of files into a collection of 16-megapixel bitmaps. Once converted those files can be placed on various photo hosting services (i.e. Google Photos unlimited storage of 16-megapixel images) for archival purposes. 

B.A.T.T. currently supports an array of options:

```
usage: bitmapallthethings
 -?,--help                     Prints this help message
 -a,--action <arg>             Sets the transcoder action. Supported
                               values are encode or decode (required)
 -b,--bytes_per_pixel <arg>    Set the number of bits per pixel. Supported
                               values are 8,16,24,32. (Default is 32)
 -c,--clean_up                 Delete temporary files.
 -e,--extension_filter <arg>   Set the extension filter
 -h,--height <arg>             Set the image height (defaults to 4000)
 -i,--input <arg>              Specifies the input target, can be either a
                               file or a folder (required)
 -m,--max_file_size <arg>      Set the max file size in bytes (defaults to
                               64000000
 -o,--output <arg>             Specifies the output directory (defaults to
                               .)
 -r,--rar                      Will attempt to execute rar if it is found
                               on the system path (valid for both encode
                               and decode).
 -rl,--rar_location <arg>      Directory were the rar executable can be
                               found.
 -rn,--rar_name <arg>          Set the name of the rar archive.
 -rp,--rar_password <arg>      Set a password and encrypt the rar files.
 -rr,--rar_recovery <arg>      Set the percentage of recovery record data
                               for rar (values are 0 - 100; default 10).
 -rx,--rar_compression <arg>   Set the amount of compression for rar
                               (values are 0 - 5; default 0).
 -s,--suppress_help            Suppresses the help output when there is a
                               command line parsing error.
 -w,--width <arg>              Set the image width (defaults to 4000)
 ```

B.A.T.T also provides a graphical user interface ("GUI") to simplify usage, it calls the command line client underneath.

![B.A.T.T. GUI](https://cloud.githubusercontent.com/assets/1129965/8385583/405b46fe-1c17-11e5-8e62-a6ef6cc7cf6b.png)

## Installation

#### Install Java: 

* [Oracle Java](http://www.java.com/en/download/); or
* [OpenJDK] (http://openjdk.java.net/)

#### Install Rar:

* [RAR](http://www.win-rar.com/download.html)

#### Download the latest release of B.A.T.T.

* [B.A.T.T.](https://github.com/tylerpitchford/bitmap-all-the-things/releases)

## Usage

It's pretty self explanitory and the default settings should be fine for most users.

If you launch the jar file with no command line options, the GUI will display. If, however, you supply command line options then the console application will process your commands.

## Compiling

#### Install Gradle: 

* [Gradle](https://gradle.org/)

#### Build the code

* `gradle build`

#### Build a complete jar

* `gradle buildFatJar`
