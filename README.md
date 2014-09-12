# ggscrape(1)

Download emails from a Google Group. Rescue your archives.

## Usage

`ggscrape <group_id> test`
check if you have permission

`ggscrape <group_id> topics`
get a list of topics

`ggscrape <group_id> messages <topic_id>`
get a list of messages in a thread

`ggscrape <group_id> download <dest_dir>`
download emails! :)

### Options

`-c, --cookie <cookie>`
Use the given cookie string. Needed to access private groups.

`-b, --begin <topicnum>`
Topic number at which to begin downloading

`-e, --end <topicnum>`
Topic number at which to stop downloading

`-l, --ln <ln_dir>`
Hard link email files into this directory. Useful for setting to a Maildir
directory, so that your local mail server can move the emails from there but
ggscrape will still know it downloaded them in the main `<dest_dir>` (in case
ggscrape is interrupted and you have to restart it.)

### Environmental variables

`GG_COOKIE`
equivalent to `--cookie`

## License

Copyright (c) 2014 Charles Lehner

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the “Software”), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
