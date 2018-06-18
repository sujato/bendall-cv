# bendall-cv
Digitization of Oskar von Hinuber’s transcription of a fragment of the Pali Cullavagga

Here we gather all the relevant information and files for the project.

In his article, von Hinuber doesn’t give a name to the manuscript, usually just referring to it as “the Nepalese fragment”. But this is too vague, and a better name is wanted. Given that multiple manuscripts may emerge from Nepal or Kathmandu, I propose we name it after Clive Bendall, who brought this fragment to light in 1899. Thus it will be "Bendall CV" or bendall-cv.

The aim is to transcribe the fragment and make it available in a segmented plain text form that can be consumed by SuttaCentral and anyone else. The process is this, more or less:

1. Type the text twice.
1. Segment it.
2. Diff it, correct, and merge.
3. Diff it once more against SC’s Mahasangiti text.

Once we are satisfied with the accuracy of the transcription, we will make it available on SC, using a custom element that enables Pali/Pali comparison with diffing against MS displayed in the browser.

## Conventions

Generally for the initial transcription we will keep it the same as the Hinuber version, and will add proper markup later.

- `[]` restored text
- `()` partly destroyed text
- `<>` text cancelled by the scribe
- `<<>>` text omitted by the scribe
- `+` obscure akṣara
- `||`, `|` dandas as in the manuscript (use upright danda rather than slash as in Hinuber).
- `//` wrap line numbers in slash
- `{}` folio numbers (no need to add PTS vol/page numbers)

## Issues with the transcription

In the scanned version of von Hinuber's text that is uploaded here, the square brackets `[` can sometimes appear like dandas `|`. Be aware that there are no straight dandas in von Hinuber's text, he only uses slash `/`. So if it looks like danda, it's a square bracket!

## Footnotes

There are a few footnotes in the transcription. These are dealt with as follows:
Folio 108b, footnote 1: Restoration not certain. In html we dealth with such issues as `class="unclear"`. I have used the notation `{{}}` for this.

## Keyboard input

An Atom package for using the Velthuis transliteration system (https://en.wikipedia.org/wiki/Velthuis) for inputting texts can be found here: https://github.com/SamaneriVimala/velthuis-autocorrect

** BE AWARE that in this text there are quotemarks that clash with the Velthuis system. So `"n` becomes `ṅ` and `"s"` becomes `ś` ** Be mindful that this can happen and correct it afterwards. The package only corrects the current word when followed by a space or linebreak.

Note that the keyboard input uses `ṁ` instead of `ṃ`. This can be kept in this text.
