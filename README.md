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

```
._ibg {
  position: relative;
  img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    object-fit: cover;
  }
}
```

for parent (with class ._ibg)
`padding-bottom: 100%;` (or hieght of image / width of image %)

Useful selectors:
```
a[href^="http"] — begins with
a[href$=".com"] — ends with


a[href*="://"] - contains letters/symbols (all outer links)
a[class~="cool"] - contains word
```


:focus-within selector
check focus-within.html and corresponding styles

When children element has focus - :focus-within (if it is set on the parent) - trigers (files in this repo ref-html) https://github.com/nk44ukrnet/html-ref

### option checked css

```
select option:default {
  color: red;
}
```

### image rendering

when scaling image -> use
`crisp-edges: crisp-edges;` - firefox  `crisp-edges: pixelated;` - chrome
