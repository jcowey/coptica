# Rules for processing

## Title of text
- Replace `\d{3}` with `P.Mon.Epiph. \1`

## Square brackets at line beginnings
- Replace `\n(\w+)\]` with `\n[.?] [\1]`
- Replace `\n\]` with `\n[.?]`

## Square brackets at line ends
- Replace `\[(\w+)\n` with `[\1] [.?]\n`
- Replace `\[\n` with `[.?]\n`

## `-` to indicate word break
- Replace `-]\n` with `]\n.- `

## Abbreviations
- Replace `(\w+)\/` with `(\1( ))`

## Dealing with `.`
- Replace `\.+` with `.x` where x= the number of dots. So `....` => `.4` make allowance for white space between dots: so `..` => `.2` but also `. .` => `.2`

## Signs
- Replace `⳨` with `*rho-cross*`
- Replace `+` with `*stauros*`
- Replace `?` with `/*?*/`
- Replace `·` with `*middot*`
- Replace `⳿` with `*word-sep-apostrophe*`
- Replace `ⲓ̈` with ` ⲓ(¨)`
- Replace `:` with `*dipunct*`


## Line numbering
- Replace `\n(\d{2})\n` with `\n\1. ` for the numerals `10|15|20` etc
- Replace `\n(\d{1})\n` with `\n\1. ` for the numeral `5`
- Replace `-\n(\d{2})\n` with `\n\1.-  ` to deal with the hypen (used to indicate the breaking of words across lines)

As a final step number all unnumbered lines from 1 through to the end of the text. 5 10 15 20 will already be correct with the above suggested change and replaces.
1.  - remember the dot whitespace 
2. 
3. 
You may of course find a much more efficient way of doing all this.
