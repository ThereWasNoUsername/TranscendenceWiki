# TranscendenceWiki
Unofficial repository of assorted documentation for Transcendence by George Moromisato

## Guidelines
Good documentation comprehensively tells you all the little details and caveats that the user wants to know about. Good documentation is well-structured.

### XML Elements
- Specify whether the element is required/optional and single/plural. We use a regex-like code to describe element counts.
  - `?`: Optional single element
  - `*`: Optional plural element
  - `1`: Required single element
  - `+`: Required plural element

### XML Attributes
- Specify the type of each attribute
  - `string`
  - `int`
  - `float`
  - etc

### Lisp Functions
- Specify the type of each argument
