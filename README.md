Fountain Tools for LibreOffice is a freeware toolset to easily create professionally formatted screenplays "from scratch," sourced from platform-independent and future-proof fountain text files (or, a subset of fountain), including proper handling of elements that span pages (no widows or orphans--it's a layout thing), and formatting which so closely mimics the better "bang for your buck" layout of Movie Magic Screenwriter that no reader will be the wiser.

For more about fountain, see: http://fountain.io or see my introduction to it in this included document:

Documentaiton.odt / .pdf

That document will also walk you through how to install and use this toolset.

This toolset also makes it relatively easy to create ebooks ready for any electronic book platform or distribution service, sourced from fountain text documents.

One additional (and not the least) feature of this toolset is to two custom, free, open-license Courier variants, Courier Mega RS (Rounded Square Slab) and SS (Square Slab) which you may like better than many others (or not). Usable exports of the fonts are included in this distribution; the development archive for those fonts is at:
https://github.com/r-alex-hall/CourierMegaFont

Finally, the provided batches fix up common screenwriting typographical errors and problems as part of formatting to screenplay.


WHAT THIS TOOLSET IS:

A major "leg up" for the spec writer or indie filmmaker: get your screenplay created in better professional form than all the other fountain-supporting software that this writer has tried, anyway (which was my motivation to create this writer's bundle). It's also convenient for ebook distribution/marketing of your script.


WHAT THIS TOOLSET IS NOT:

This is not a film production replacement for professional screen layout software. If your screenplay heads into production, you or the folks you sell your screenplay to will want the software toys which all the "big boys" use for production, revision and budgeting etc. features. Fortunately, when you get to that stage, your fountain text screenplay sources will easily import into those more expensive toys. Meanwhile, you have no need for those (expensive, proprietary, closed-source, restrictive-license, platform-dependent) toys. In other words, this toolset is a free and convenient stop-gap for the professional or aspring "spec" writer.


THIS TOOLSET CONTAINS:

	1) "LibreOffice_ScreenplayTemplate_v1.3.4.2 (standard).odt":
	An OpenOffice/LibreOffice template with styles to easily format plain text documents as proper screenplays (industry-standard complaint). Yes, there's another template out there already that does this. This one is better because it gets more "bang for the buck" with space: it very closely follows the formatting and layout "cheats" of Movie Magic Screenwriter, which gets more words on a page with no one the wiser. (My apologies to Final Draft fans: I simply haven't examined the thing. Much.)

	2) "AltSearchScript Fountain Batch 1.2.txt":
	Source code which can easily be copied (see documentation.pdf) into the batch source file of one Alt.Search-Replace LibreOffice extension, to allow batch conversion of fountain text to a properly formatted screenplay (by way of the provided document template with screenplay styles).

	3) "libreOfficeExtension_AltSearch-1.4.oxt":
	A copy of said LibreOffice extension for you to install (you may find the same or a newer version of the extension with an internet search for "LibreOffice Alt.Search-Replace extension" (which is, like LibreOffice itself, freely sourced and licensed).

	4) In the /fonts folder:
	Copies of fonts developed by me to solve problems described at the repository referenced earlier in this document.

	Last but not least, this toolset is freely sourced (GNU GPL v3 or later) and platform-independent; anywhere that you can install LibreOffice, you can install this toolset, and you may also freely adapt/redistribute this toolset for your own purposes.


MORE EXPLANATION

Problems this toolset solves:

SOLVED PROBLEM: there are several applications which support fountain for import, conversion, and/or export to and from various formats, but none of them have consistently bridged well from Fountain to Movie Magic Screenwriter, that I have tried. Moreover, they have inconsistently recognized text imported or copied from any Open Document Text (such as you can create in Libre Office), or Microsoft Word text either, for that matter. It's *possible* they may import better from .odt docuements provided by this toolset.

SOLVED PROBLEM: there wasn't anything "on the market" (that I've found) which easily bridges fountain (and for that matter screenplays in general) to ebooks. This toolset solves that problem gracefully and with relatively little fuss.

SOLVED PROBLEM: No truly open-source and free Courier fonts to my liking existed. See notes in the README.md of the font repository referenced at the start of this document.

SOLVED PROBLEM: No truly libre toolset "on the market" that "cheats" layout and elements as expertly as Movie Magic Screenwriter does (which it does, by the way), to get the mentioned page-count "bang for your buck", AND nothing libre on the market (that I remember? Though I could be wrong) which properly handles widow/orphan control for elements. The provided template handles those, or properly paginates of elements: for example character headers, parentheticals, and scene headers will never be split accross different pages, they will always remain grouped with dialogue, and dialogue that takes more than two rows of text will be pushed to the next page.

You're welcome :)

08/12/2014 12:50:00 AM -Richard Alexander Hall
http://www.earthbound.io/contact

VERSION HISTORY


08/12/2014 12:50:15 AM INITIAL RELEASE
Bada-bing! :) But the fonts in this release are alpha-quality, with only two weights provided--what I regard as my preferred "regular" and also a black variant for each mentioned family. ALSO, importantly there are not (in this release) any italic, bold, or bold italic variants--so that disappointingly, sometimes software makes no visual distinction between the regular and a faked bold for these. I'm actually happy enough with Courier Prime. Almost. It's too fat and roundy. Can you see why I might want to be an amateur font designer, at least? :) But Courier Prime did great stuff with their approach to more legible italics. AND my template and these documents use it at initial release of this. The font dev sources I provide are to spur anyone else who may have interest. But I may work them up further myself.