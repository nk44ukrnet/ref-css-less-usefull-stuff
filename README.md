# ref-css-less-usefull-stuff

Responsive font size.
Can be used inside (max-width), (min-width)

``.font-fluid(@min, @max) {
  font-size: calc(@min*1px + (@max - @min) * ((100vw - 320px) / (1200 - 320)));  
}``
