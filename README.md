# README for karauke_udn songsheets

This is a repo for songsheets in _ukedown_ format. This is a plain text format,
a special case of the commonly used 'markdown' format.

With the appropriate tooling it can be converted into HTML, EPUB and/or PDF for
publication, projection etc, using CSS for styling.

## How to contribute/submit changes etc

Before you can do this you will need an account on github.

A brief intro to editing with git is in [EDITING.md](EDITING.md)

Alternatively you can find info about editing directly in the github web
interface in [ONLINE_EDITING.md](ONLINE_EDITING.md)

## ukedown format

Ukedown looks a great deal like the
[ukulele wednesdays](http://ukulelewednesdays.com) format, because that's where
it started. The following formatting is supported


### 1. Artist and Title

The first non-blank like in a ukedown file should contain TITLE - ARTIST.
Or just TITLE if there is no artist, or it's unknown.

    Rolling in the Deep - Adele

This will  be rendered in the output like this:
**Rolling in the Deep - Adele**

### 2. Chords

Chords are displayed inline, surrounded by parentheses. Just like the wednesdays
format, without worrying about making them **bold**

    (Bb)Don’t underestimate the (Gm)things that I will (Bb)do

- No funny business like 'Single Strums' or unicode downarrows'

### 3. Sections

Section titles should be surrounded by square brackets, e.g. `[chorus]`, which
are then rendered as second-level headers, like this:

**[chorus]**

### 4. Performance Notes
You know, things like 'quietly', 'single strums', 'a capella' etc

Written like this:

    {quietly}
    {stop backing vox}

Rendered like this:

<b>[quietly]</b><br/>
<b>[stop backing vox]</b>

Unlike headings, these can be displayed on the same line as other elements, so
they can go at the end of lines etc.

### 5. Backing Vocals

Backing vocals are written like chords, using parentheses.
This may change in a future revision as it could potentially lead to confusion.

Currently anything surrounded by `(` and `)` that doesn't match a known chord
pattern is presumed to be backing vocals.

    (Cm)(You’re gonna wish you) (Bb)(never had met me)

(which has both chords and vocals) renders like this:

<b>(Cm)</b><i>(You’re gonna wish you)</i> <b>(Bb)</b><i>(never had met me)</i>

An example with chords, normal vox and backing vox:

    (G7)Oh, (C)oo-bee-doo (oop-de-wee)
    I wanna be like (A7)you (hup-de-hooby-do-bah)

Which should produce this:

<b>(G7)</b>Oh, <b>(C)</b>oo-be-doo <i>(opp-de-wee)</i><br/>
I wanna be like <b>(A7)</b>you <i>(hup-de-hooby-do-bah)</i><br/>

### 6. Boxed sections

Repeated song sections, such as choruses and bridges are often put into boxes,
to avoid repetition.

In ukedown this is done using the _pipe_  character, `|` at the beginning of
each line you want in a box.
You can put them at the end too, if you want, but it's not required.

By which I mean

    |[chorus]
    |We could have had it (Cm)Aa-aa-(Bb)all
    |rolling in the (Ab)Dee-ee-(Bb)eep

is exactly the same as

    |[chorus]                               |
    |We could have had it (Cm)Aa-aa-(Bb)all |
    |rolling in the (Ab)Dee-ee-(Bb)eep      |

and results in something like this (style-dependent)

<table border="1px solid black" padding="5px" width="80%" margin-left="5%">
<tr>
<td>
<h2>[chorus]</h2>
We could have had it <b>(Cm)</b>Aa-aa-<b>(B&flat;)</b>all</br>
rolling in the <b>(A&flat;)</b>dee-ee-<b>(B&flat;)</b>eep
</td>
<tr>
</table>

<!-- vim: se nofen tw=80: -->
