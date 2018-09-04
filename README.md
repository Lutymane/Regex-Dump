# Regex-Dump

Dump of regex expressions made by me for various needs

## Match YouTube links and get video id


```javascript
//str stores text containing yt link
var str = 'anytext http://www.youtube.com/watch?v=sassd21d1-_2d boop';
var rgx = /https?:\/\/(?:www\.)?youtu(?:\.be\/([-A-Za-z0-9_]+)|be\.com\/watch\?v=([-A-Za-z0-9_]+)(?:&.+)?/g;
var arr = rgx.exec(str);
var id = arr[1] || arr[2];
//id stores yt video id
```
