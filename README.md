# ref-css-less-usefull-stuff

``.font-fluid(@min, @max) {
  font-size: calc(@min*1px + (@max - @min) * ((100vw - 320px) / (1200 - 320)));  
}``

Responsive font size.

Can be used inside (max-width), (min-width)
