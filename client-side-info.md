Client side decompression (extracts and runs in your web browser without need of a server) is useful for places without server side compression like blogs, cell phone applications, free hosting spots, storing local self extracting/executable web pages, standalone web page applications in HTML5 and more. It can also come in handy for embedding codes to HTML, escaping codes for HTML/JavaScript, encoding code (why bother with base64 encoding that makes everything 30% bigger, use our bzip packer instead for 50% smaller), hosting where you are limited space and/or bandwidth (server and/or get twice as much on a 10MB free web host), obfuscating your source codes (major obfuscation on www.whak.ca main page, but not compressors) and much more...

Images, JavaScript & CSS can be embedded right into a single webpage (less calls to external files means better performance)

Online tools to create your own client side compressed files:

www.whak.ca/packer/JavaScript.htm
www.whak.ca/packer/HTML.htm
www.whak.ca/packer/CSS.htm
www.whak.ca/packer/PNG.htm
www.whak.ca/packer/ASP.htm
www.whak.ca/packer/PHP.htm

Here is a demo of the PNG packer: http://jsfiddle.net/6px7yru0/show/ It's a real PNG image compressor from a compiled C++ programmed application converted using Emscripten to bytecode/Web Assembly. At first it was 2.8 MB, but I compressed it for client side (built in decompressor) to 614 KB, gzip gets 590KB, so it's pretty damn close! I could get get better results using bzip with the HTML packer (around 500KB), but this one extracts much faster

Here are some live unpacking speed tests:

www.whak.ca/speed-test.htm

https://github.com/JavaScript-Packer/jquery-bzip-compressed (smallest in the World) has some sample JQuery files that I compressed to less than half the size than even the "min" versions offered on JQuery.com. See http://jsfiddle.net/nk6Lryos/ for a 18KB Hello World demo that has a complete JQuery file embedded. If Microsoft or Google were to use those files instead on their CND, they would save thousands of dollars on bandwidth every week and terrabytes of wasted data.
