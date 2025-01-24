# Rules for processing

## Title of text
- Replace `\d{3}` with `P.Mon.Epiph. \1`

## Line numbering
- Replace `\n(\d{2})\n` with `\n\1. ` for the numerals `10|15|20` etc
- Replace `\n(\d{1})\n` with `\n\1. ` for the numeral `5`
- Replace `-\n(\d{2})\n` with `\n\1.-  ` to deal with the hypen (used to indicate the breaking of words across lines)

## Square brackets at line beginnings
- Replace `\n(\w+)\]` with `\n[.?] [\1]`
- Replace `\n\]` with `\n[.?]`

## Square brackets at line ends
- Replace `\[(\w+)\n` with `[\1] [.?]\n`
- Replace `\[\n` with `[.?]\n`

## ``-` to indicate word break
- Replace `-]\n` with `]\n.- `

## Signs
- Replace `⳨` with `*rho-cross*`
- Replace `+` with `*stauros*`
- Replace `?` with `/*?*/`
- Replace `·` with `*middot*`
- Replace `⳿` with `*word-sep-apostrophe*`
- Replace `ⲓ̈` with ` ⲓ(¨)`
