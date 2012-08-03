Ghostscript Fonts
=================

The URW Ghostscript fonts are a set of open source Fonts created by the type
foundry URW that are made to match the 35 fonts in the PostScript
specification.

A list of the fonts contained and the fonts they are inspired on:

Bookman L -> Bookman
Century Schoolbook L -> New Century Schoolbook
Chancery L -> Zapf Chancery
Dingbats -> Zapf Dingbats
Gothic L -> Avant Garde
Nimbus Mono L -> Courier
Nimbus Roman No9 L -> Times
Nimbus Sans L -> Helvetica
Palladio L -> Palatino
Standard Symbols L -> Symbol

source: http://en.wikipedia.org/wiki/Ghostscript#Free_fonts

For this release the PostScript fonts from the SourceForge project
http://sourceforge.net/projects/gs-fonts/ have been converted to UFO’s, 

They are pretty complete, but the original todo’s stand:

-   fix all missed glyphs.
-   change suitable glyphs with references.
-   improve bearings of glyphs (thanks Dmitry 40in who pointed to this)
-   improve outlines of some cyrillic glyphs

Especially #2 makes sense when building on these fonts: right now a, á, ä and 
â all contain a seperate a, and î and û contain a separate ˆ. Not easy to 
maintain, it is better if there is one a and the rest is changed into 
references.

Finally a proper LICENSE.txt should be added.

Original README
---------------

This is release 1.0.7pre22 of Valek Filippov's improved versions of the URW
type 1 font collection, repackaged for distribution with Ghostscript.

Cyrillized free URW fonts.

These fonts were made from the free URW fonts distributed with ghostcript.
There are NO changes in the latin part of them (I hope).
Cyrillic glyphs were added by copying suitable latin ones
and painting oulines of unique cyrillic glyphs in same style as the others.
For all modification pfaedit was used.
The license for result is (of course) same as for original fonts,
i.e. GPL with an exception that you can put these fonts in your own non-GPLed
documents. (Looks like LGPL from my point of view =).

The "sources" of these fonts in the native pfaedit format are available
at ftp://ftp.gnome.ru/fonts/sources

The great font editor pfaedit is available at http://pfaedit.sf.net.
That page also includes some links to fonts created by
George Williams -- the author of pfaedit.

Acknowledgements:
I would like to thank George Williams, the pfaedit's author and developer.
He is the most bug-reporter/feature-requester friendly developer
I ever saw in my not so short life. At some moment in the future
I must write a book about him: "George Williams and my best experience
in bug-reporting." George also greatly helped me bug-hunting these fonts,
explained to me some very important things about fonts and font design,
quickly adopted pfaedit to my needs (or pointed me to The Right Place in
documentation where I found better way of doing things).

I would like to thank Alexey Novodvorsky (aka AEN), who
pointed me to pfaedit and George Williams' fonts, explained
The Task to me. He is also one of the main participators in the
development of Sysiphus -- free repository of free software.
I didn't loose my time for compiling/installing and supporting
my linux box coz I used the result of Sysiphus developers' works.

I would like to thank Sergey Vlasov, who tested these fonts and reported
about bugs. Also he help me to make some bug-reports to George about
pfaedit bugs.

I would like Dmitry 40in, who did big QA for some font outlines, drawn some glyphs,
and explain some The Truths for me.

I would like to thank Vlad Harchev (aka hvv), who
proofread this text for me.

Also I have to thank RMS for GPL and URW for releasing the fonts
under it.

Thank you very much!
Valek Filippov frob@df.ru
(C)opyLeft 2001

Original README.tweaks
----------------------

Nimbus Sans L Regular, Nimbus Mono L Regular, Nimbus Mono L Oblique
all come from a more recent version of the cyrillic URW fonts.

The hints on Nimbus Sans Regular have been modified in the
following ways:

25 June 2002

 - Added ghost hint to the top of 4 to keep it from being
   taller than the other digits.
 - Reduced the width of the left stem hint for H to 83
   (probably no real differences)
 - Changed the StemSnapV values from [78 85 94] to [78 83 92]
   (and fixed up StdVW accordingly)
   This corresponds to the values in the font (which are 83/93
   for lower case and upper case stems) better and makes
   the width-88 stems on M and N snap to to upper case 
   widths not lower-case widths.

29 June 2002

 - Removed odd vertical stem hints (width of horizontal
   stems) from f, F, t, E, yen sign, fi ligature, 
   fl ligature, AE ligature, R, Lstroke, OE ligature,
   lstroke, E" variants, t, variants, Eth, Dstoke, etc.
 - Fixed hints on 1 to be two ghost hints instead of one
   hint the height of the font
 - fix bottom stem of u to have integer coordinates
 - fixed hints on |
 - fixed hints on inverted exclamation mark

The hints on Nimbus Mono L Oblique have been modified in the
following ways:

 - Removed vertical stem hints from horizontal serifs on
   roman characters.
  
Owen Taylor

