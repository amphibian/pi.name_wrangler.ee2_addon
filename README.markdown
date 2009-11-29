Name Wrangler lets you use proper names in the format SURNAME, GIVEN NAME in the back-end (in order to faciliate proper sorting), but still display them in the the format GIVEN NAME SURNAME. It also allows you to display first, middle, and last names independently, in both singular and posessive forms, and to do this with both individual names and lists of ampersand- or semicolon-separated names.

##Parameters:

- **type**: the type of name(s) to return. Either "full", "first", "middle", "first+middle", or "last".  Defaults to "full".
- **form**: either "singular" or "posessive". Defaults to "singular".
- **and**: word or character entity to use  before the last name at the end of a list of names.  Defaults to "&amp;".

##Example use:

`{exp:name_wrangler}Hedges, Chris{/exp:name_wrangler} consistently impresses me with his writing and journalism.`

Returns "Chris Hedges consistently impresses me with his writing and journalism."

`{exp:name_wrangler type="first" form="posessive"}Hedges, Chris{/exp:name_wrangler} latest book is a sobering read.`

This returns "Chris' latest book is a sobering read."

`{exp:name_wrangler type="last"}Hedges, Chris & Moore, Alan & Robinson, Kim Stanley{/exp:name_wrangler} are very different, but all must-read authors.`

This returns "Hedges, Moore & Robinson are very different, but all must-read authors."

##Compatibility

This version of Name Wrangler is compatible with ExpressionEngine 2.0 and higher. The ExpressionEngine 1.6-compatible version [can be found here](http://github.com/amphibian/pi.name_wrangler.ee_addon).
