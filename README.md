# bendall-cv
Digitization of Oskar von Hinuber’s transcription of a fragment of the Pali Cullavagga

Here we gather all the relevant information and files for the project.

In his article, von Hinuber doesn’t give a name to the manuscript, usually just referring to it as “the Nepalese fragment”. But this is too vague, and a better name is wanted. Given that multiple manuscripts may emerge from Nepal or Kathmandu, I propose we name it after Clive Bendall, who brought this fragment to light in 1899. Thus it will be "Bendall CV" or `bendall-cv`.

The aim is to transcribe the fragment and make it available in a segmented plain text form that can be consumed by SuttaCentral and anyone else. The process we used was this:

1. Type the text twice, with two different typists (Venerables Vimala and Sunyo).
1. Segment it, using the Mahasangiti as a reference.
1. Diff the two typed versions, correct, and merge.
1. We found that several glyphs were unclear due to poor quality scans, so we had the original article rescanned at this point. The master file was then checked once more against the new scan.
1. Diff the bendall-cv against the sanitized text produced from SC’s Mahasangiti text, resolving any differences by referring to the new scans.

Once we are satisfied with the accuracy of the transcription, we will make it available on SC, using a custom element that enables Pali/Pali comparison with diffing against MS displayed in the browser.

## The files

- `bendall-cv2.tx` and `bendall-cv-3.txt` are the raw typed files. They should not be corrected further.
  - Now deleted!
- `pli-tv-kd14.html` and `pli-tv-kd15.html`are the Mahasangiti files as used on SC.
- The `segmented` files have been segmented so as to match up as well as possible.
- `bendall-cv.txt` is the master file for the text. It was created by comparing the differences in the above and checking with von Hinuber's edition. Future corrections should be done to this.
- The `sanitized` versions have had all punctuation, capitals, references, and apparatus removed. These are for diffing. If `bendall-cv.txt` is corrected, the corresponding `sanitized` file should be updated.

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

## Keyboard input

An Atom package for using the Velthuis transliteration system (https://en.wikipedia.org/wiki/Velthuis) for inputting texts can be found here: https://github.com/SamaneriVimala/velthuis-autocorrect

** BE AWARE that in this text there are quotemarks that clash with the Velthuis system. So `"n` becomes `ṅ` and `"s"` becomes `ś` ** Be mindful that this can happen and correct it afterwards. The package only corrects the current word when followed by a space or linebreak.

Note that the keyboard input uses `ṁ` instead of `ṃ`. This can be kept in this text.

## Possible errors and comments on the manuscript

- Folio 107a/4b/ bhaṇḍanajātanaṁ should probably be bhaṇḍanajātānaṁ as elsewhere in the transcription. Corrected in master. (The ā in question seems to have a macron *below* it in Hinuber's book. I guess it's a printing error. Perhaps check against Devanagari ms.)
- Folio 108b/3c/ one danda missing between `tha | pka` (not corrected)

Then in several places in the script (I counted 6), as outlined on page 9, there is a letter m̄ (m with macron). It is not certain what this means and Ven. Anandajoti had never seen it used before either. I have just kept it in as is.

There are a few footnotes in the transcription. I have not added these but they might need to be added. One I have added additional coding for: Folio 108b, footnote 1: Restoration not certain. In html we dealt with such issues as `class="unclear"`. I have used the notation `{{}}` for this.
