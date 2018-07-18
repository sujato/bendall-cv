# bendall-cv
Digitization of Oskar von Hinüber’s transcription of a fragment of the Pali Cullavagga.

Here we gather all the relevant information and files for the project. The aim is to transcribe the fragment and make it available in a segmented plain text form that can be consumed by SuttaCentral and anyone else. This is purely a digitization of von Hinüber’s transcription and we have not referred to the original.

In his article, von Hinüber doesn’t give a name to the manuscript, usually just referring to it as “the Nepalese fragment”. But this is too vague, and a better name is wanted. I propose we name it after Clive Bendall, who brought this fragment to light in 1899. Thus it will be “Bendall Cullavagga” or `bendall-cv`.

The process we used was this:

1. Type the text twice, with two different typists (Venerables Vimala and Sunyo). ☑
1. Segment it, using the Mahāsaṅgīti as a reference. ☑
1. Diff the two typed versions, correct, and merge. ☑
1. We found that several glyphs were unclear due to poor quality scans, so we had the original article rescanned at this point. The master file was then checked once more against the new scan. ☑
1. Diff the bendall-cv against the sanitized text produced from SC’s Mahāsaṅgīti text, resolving any differences by referring to the new scans. ☑

While we are confident that the transcribed text is accurate, such work is never perfect, so we welcome any additional corrections.

In due course we will make it available on SC, using a custom element that enables Pali/Pali comparison with diffing against MS displayed in the browser.

## The files

- `bendall-cv.txt` is the master file for the text.
- `pli-tv-kd14.html` and `pli-tv-kd15.html`are the Mahāsaṅgīti files as used on SC.
- The `segmented` files have been segmented so as to match up as well as possible.
- The `sanitized` versions have had all punctuation, capitals, references, and apparatus removed. These are for diffing.
- The `images` folder contains the scanned images of the text in latin and devanagari scripts.
- The `related-articles` folder contains the original article by von Hinüber.

## Conventions

Generally for the initial transcription we keep it the same as the von Hinüber version.

- `[]` restored text
- `()` partly destroyed text
- `<>` text cancelled by the scribe
- `<<>>` text omitted by the scribe
- `+` obscure akṣara
- `||`, `|` daṇḍas as in the manuscript (use upright daṇḍa rather than slash as in von Hinüber).
- `//` wrap line numbers in slash
- `{}` folio numbers (no need to add PTS vol/page numbers)
- `{{}}` uncertain restoration

## Keyboard input

An Atom package for using the Velthuis transliteration system (https://en.wikipedia.org/wiki/Velthuis) for inputting texts can be found here: https://github.com/SamaneriVimala/velthuis-autocorrect

- In this text there are quotemarks that clash with the Velthuis system. So `"n` becomes `ṅ` and `"s"` becomes `ś` Be mindful that this can happen and correct it afterwards. The package only corrects the current word when followed by a space or linebreak.
- Note that the keyboard input uses `ṁ` instead of `ṃ`.

## Notes

- Folio 107a/4b/ bhaṇḍanajātanaṁ should probably be bhaṇḍanajātānaṁ as elsewhere in the transcription. Corrected in `bendall-cv.txt`.
- Folio 108b/3c/ one daṇḍa missing between `tha | pka`. Corrected in `bendall-cv.txt`.
- In 7 places in the script there is a letter m̄ (m with macron), described by von Hinüber (p. 9) as “miniature *akṣaras* the meaning of which cannot always be established.” It is a kind of *anusvāra*, so it may be best to simply replace with ṁ. However we have left it for the time being.
- There are a few footnotes in the transcription. We have incorporated the gist of one note in the text: page 34, Folio 108b/3c, footnote 1: “Restoration not certain. Either as above following Ee, or [mallake]na na.” We have used the notation `{{}}` for this. In SuttaCentral html we dealt with such issues as `class="unclear"`.
