#No documentation yet!
(feel free to write a bit about it)

You can check for `btoa` and `atob` support and refer to `jQuery.base64`

    if (!window.btoa) window.btoa = $.base64.btoa
    if (!window.atob) window.atob = $.base64.atob

## Options
You can define some options per default, set them globally use the following syntax:

`$.base64.utf8encode = true;`

Utf8 encoding and decoding as global option, possibilities:

| option | description | default |
|:--|:--|:--|
| `raw` |  If `false` it encodes/decodes both, the input and output. | `true` |
| `utf8encode` |  To encode only the input you can set encodung to `true`. | `false` |
| `utf8decode` | Same as above but for the output and decoding. | `false` |

You can override the global options by passing an extra parameter:

`$.base64[property](<value>, options);` / `$.base64(<property>, <value>, options);`

To enable `UTF8-encoding` pass true as the last paramter:

    $.base64.atob(<value>, true);
    $.base64('atob', <value>, true);

## Download
Get the [raw](https://raw.github.com/yckart/jquery.base64.js/master/jquery.base64.js) script, download the complete [package](https://github.com/yckart/jquery.base64.js/zipball/master) or fork it on [GitHub](https://github.com/yckart/jquery.base64.js/).

## Support

 [@yckart](http://twitter.com/yckart) #jquery #base64
 [http://yckart.com](http://yckart.com/)

### Thanks
- https://github.com/carlo/jquery-base64

###License
Copyright (c) 2013 Yannick Albert ([http://yckart.com/](http://yckart.com/))

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
