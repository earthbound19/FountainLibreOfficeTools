# Fountain Tools for LibreOffice
Free and open source (libre) software that converts any plain text [fountain format screenplay](http://fountain.io) to an industry standard layout document, and does better at this than all other FOSS tools. Output is on par with proprietary software, and with a custom libre font (linked to and also developed by me), even better. An additional novelty feature is ebook-friendly export.

# Features
I could not find any tools "on the market" which solve all of the following problems and have all the following features. This toolset does and solves these problems:

- Creates industry standard output with future-proof plain text files and libre software, without monetary license and proprietary restrictions
- Intermediate output is .odt (Open Document Text), which may be exported to .pdf
- Uses a subset of fountain format which discards all features you don't need. If you think you need them, your formatting and writing is too elaborate: you can accomplish everything more simply.
- No other libre toolset "cheats" layout and elements and does layout as expertly as Movie Magic Screenwriter:
 - Widow/orphan control for elements. The templates in this toolset do this. Elements such as character headers, parentheticals, and scene headers will never be split across different pages: they will always remain grouped with dialogue, and dialogue that takes more than two rows of text will be pushed to the next page.
 - More words on a page without cramping, which reduces page count
- No other toolset easily bridges fountain (or screenplays in general) to ebooks. This toolset does so gracefully.
- Fixes typographical and layout errors when it formats, including imposition of technical opinions. For example, you may not want to mix (O.S.) (O. S.) and (V.O.) -- they can and should all just be (V.O.)
- Option to globally change screenplay font
- While at least several other tools (when this tool was developed) support fountain import, conversion, and/or export to and from various formats, none of them consistently bridge well from Fountain to Movie Magic Screenwriter. They moreover inconsistently recognize text imported or copied from any Open Document Text (such as you can create in Libre Office), or Microsoft Word for that matter. It's possible those tools will import better from .odt documents created by this toolset.
- (Became a separate, now finished task) No other libre Courier fonts to my liking exist. Particularly for a necessarily information-heavy screenplay (such as science fiction), the following libre fonts will get more characters on a page; see the [Courier Mega font repository](https://github.com/r-alex-hall/CourierMegaFont) or as released [at sourceforge](http://fountainlibreofficetools.sourceforge.net).
- Visual and written installation and usage guide (see `Documentation.pdf`)

# What this toolset is not
This toolset is suitable for spec writing, but not production. When you get into production you'll want to buy and use proprietary tools that coordinate a screenplay with logistics and production.

## Toolset items

- `LibreOffice_ScreenplayTemplate_vx.x.x.x (standard).odt` is an OpenOffice/LibreOffice template with styles to easily format plain text to industry standard screen format (as detailed under "Features").
- `AltSearchScript Fountain Batch 1.x.txt,` is batch source code for the the Alt.Search-Replace LibreOffice extension, which searches for fountain regex patterns and applies the screen format document styles of the screenplay template to them. See `documentation.pdf` for instructions.
- `libreOfficeExtension_AltSearch-x.x.oxt` is a copy of said LibreOffice extension for you to install.

## To do
Adapt documentation to markdown with source images in repo, ditch cumbersome .odt / .pdf

## Contact
http://www.earthbound.io/contact

VERSION HISTORY

2018-09-04 09:51:29_AM 
- Edited README.md for brevity/clarity including merging redundant sections/lists.
2018-06-13 08:40:38 AM
- Update included Alt Search Libre Office extension to v1.4.2
- Deleted template pdf (why was that there?)
- Overhauled README.md
- Deleted from template a reference to a font which will be nonexistent unless folks install my custom screenplay font. (A previous push claimed I did this, but it seems to me I didn't push the change.)

2014-09-05 05:53:56 PM
Commit experimental tweak batch to conjoin improperly broken (e.g. from HTML) paragraphs. Edit outdated info out of version history (re included font--it's not included anymore, but linked to).

2014-08-18 05:07:23
- Bug fix: some elements did not inherit font styles from the default screenplay style (e.g. transitions or scenes could be bold after changing the default font, where they should be regular, if the default font is regular). Fixed by going into the properties of each element style, on the font tab, and clicking "standard," then "apply."

2014-08-12 12:50:15 AM
Initial release