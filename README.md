# ref-css-less-usefull-stuff 


(fluid font sizes)

Responsive font size.
Can be used inside (max-width), (min-width)

``.font-fluid(@min, @max, @maxWidth: 1200) {
  font-size: calc(@min*1px + (@max - @min) * ((100vw - 320px) / (@maxWidth - 320)));
}``
