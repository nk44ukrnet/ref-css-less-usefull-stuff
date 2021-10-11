# ref-css-less-usefull-stuff 


(fluid font sizes)

Responsive font size.
Can be used inside (max-width), (min-width)

```
.font-fluid(@min, @max, @maxWidth: 1200) {
  font-size: calc(@min*1px + (@max - @min) * ((100vw - 320px) / (@maxWidth - 320)));
}
```


(fluid images)

```._ibg {
  position: relative;
  img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    object-fit: cover;
  }
}```

for parent (with class ._ibg)
`padding-bottom: 100%;` (or hieght of image / width of image %)
