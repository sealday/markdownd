Markdownd
================

This project is forked from [instant-markdown-d](https://github.com/suan/instant-markdown-d).

markdownd is a small Node.js server that enables instant compilation and previewing of Markup files. 
A plugin can easily be written for any text editor to interface with it. One currently exists for 
VIm: https://github.com/suan/vim-instant-markdown

Feature
-------

- realtime preview (origin feature)
- support emoji
- synchronized scroll

Installation
------------
- `[sudo] npm -g install markdownd`

REST API
--------
| Action                   | HTTP Method | Request URL               | Request Body                   |
|--------------------------|-------------|---------------------------|--------------------------------|
| Refresh Markdown on page | PUT         | http://localhost:\<port\> | \<New Markdown file contents\> |
| Close Webpage            | DELETE      | http://localhost:\<port\> |                                |

By default, `<port>` is 8090
