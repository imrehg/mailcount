Mail Counter
============

Count the number of emails in a day across multiple email accounts,
in specific folders (or "mailboxes").

Config file example
-------------------

Save a file for configuration in Python's ConfigParser format,
where every section is a new mailbox, the section header is used as
a "friendly name", the section should contain `server`, `login`,
`pass`, and `mailbox` parameters. Can have as many sections, i.e.
mailboxes as you like, as long as they have different friendly names

```
[Personal Gmail]
server=imap.gmail.com
login=myemail@gmail.com
pass=totallysecretpassword
mailbox=[Gmail]/Sent Mail
```

Experience
----------

If you can, use "application specific password" on Gmail, so if your
configuration file falls in the wrong hands, you can just revoke access.

The `mailbox` is the trickiest to figure out, on Gmail I've seen seen
`[Gmail]/` or `[Google Mail]/` prepended to the label's name to give its
IMAP name that can be used.

License
-------

The MIT License (MIT)

Copyright (c) 2014 Gergely Imreh <gergely@imreh.net>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.