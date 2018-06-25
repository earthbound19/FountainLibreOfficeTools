# Fountain Tools for LibreOffice
Freeware that converts any plain text [fountain format screenplay](http://fountain.io) to an industry standard layout document, and does better at this than all other FOSS tools. Output is on par with that from proprietary software (and with a custom, FOSS font, even better). An additional novelty feature is ebook-friendly export.

# Features
- Create industry standard output with future-proof plain text files and free, open source software, without monetary license and proprietary restrictions
- Intermediate output is .odt (Open Document format), which may be exported to .pdf
- Visual and written installation and use guide (see `Documentation.pdf`)
- Uses a subset of fountain format which discards all features you don't need (if you think you need them, your formatting and writing is too elaborate: you can accomplish everything more simply).
- Mimics Movie Magic Screenwriter output that fits more words on a page without cramping (this means lower page count)
- Layout avoids widows and orphans (where other free tools don't)
- Alternate ebook output
- Fixes up common screenplay typographical errors when it formats. For example, you would be wrong to mix (O.S.) (O. S.) and (V.O.) -- they can all and should all just be (V.O.)
- Optionally globally change screenplay font (a font referenced in this documentation will tighten up presentation further without cramping it)

If you write a necessarily information-heavy screenplay (such as science fiction), you may wish to get yet more characters on a page via any of the libre fonts at the [Courier Mega font repository](https://github.com/r-alex-hall/CourierMegaFont) or as released [at sourceforge](http://fountainlibreofficetools.sourceforge.net).

# What this toolset is not
This toolset is suitable for spec writing, but not production. When you get into production you'll want to buy and use proprietary tools that coordinate a screenplay with logistics and production.

## Toolset items

- `LibreOffice_ScreenplayTemplate_v1.3.4.2 (standard).odt` is an OpenOffice/LibreOffice template with styles to easily format plain text to industry standard screen format. Yes, there's another template out there, but this one mimics the tighter layout of Movie Magic Screenwriter, and avoids widows and orphans.
- `AltSearchScript Fountain Batch 1.x.txt,` is batch source code for the the Alt.Search-Replace LibreOffice extension which searches for fountain regex patterns and applies the screen format document styles of the screenplay template to them. See `documentation.pdf` for instructions.
- `libreOfficeExtension_AltSearch-1.4.oxt` is a copy of said LibreOffice extension for you to install.

## To do
Adapt documentation to markdown with source images in repo, ditch cumbersome .odt / .pdf

## Developer notes
- SOLVED PROBLEM: there are several applications which support fountain for import, conversion, and/or export to and from various formats, but none of them have consistently bridged well from Fountain to Movie Magic Screenwriter, that I have tried. Moreover, they have inconsistently recognized text imported or copied from any Open Document Text (such as you can create in Libre Office), or Microsoft Word text either, for that matter. It's *possible* they may import better from .odt docuements provided by this toolset.
- SOLVED PROBLEM: there wasn't anything "on the market" (that I've found) which easily bridges fountain (and for that matter screenplays in general) to ebooks. This toolset solves that problem gracefully and with relatively little fuss.
- SOLVED PROBLEM: No truly open-source and free Courier fonts to my liking existed. See notes in the README.md of the font repository referenced at the start of this document.
- SOLVED PROBLEM: No truly libre toolset "on the market" that "cheats" layout and elements as expertly as Movie Magic Screenwriter does (which it does, by the way), to get the mentioned page-count "bang for your buck", AND nothing libre on the market (that I remember? Though I could be wrong) which properly handles widow/orphan control for elements. The provided template handles those, or properly paginates of elements: for example character headers, parentheticals, and scene headers will never be split accross different pages, they will always remain grouped with dialogue, and dialogue that takes more than two rows of text will be pushed to the next page.

## Contact
http://www.earthbound.io/contact

VERSION HISTORY

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