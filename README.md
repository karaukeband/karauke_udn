# README for karauke_udn songsheets

This is a repo for songsheets in //ukedown// format. This is a plain text format, a special case of the commonly used 'markdown' format. With the appropriate tooling it can be converted into HTML, EPUB and/or PDF for publication, projection etc, using CSS for styling.

## ukedown format

Ukedown looks a great deal like the /ukulele wednesdays/ format, because that's where it started. The following formatting is supported

  * The first non-blank like in a ukedown file should contain TITLE - ARTIST. or just TITLE if there is no artist, or it's unknown.
  * Chords are displayed inline, surrounded by parentheses. For example, `(C)` or `(Asus4). No funny business like 'Single Strums' or unicode downarrows'
  * Section titles are surrounded by square brackets, e.g. `[chorus]`
  * performance notes (like 'single strums' or 'stop playing' or anything else, really) are denoted by curly braces, like this `{single strums}`
  * backing vocals are currently also surrounded by () - this may change. Anything that doesn't match a known chord pattern but is contained in parentheses will be rendered as backing vocals
  * box sections (for repeated choruses etc) are created by starting all the lines you want in the box with a '|'

## format limitations
