# README

One of the great advantages of the segmented text approach that we use here is that it allows easy and precise diffing. This folder is to demonstrate how this works as a proof-of-concept.

Github shows diffs for versions of the same file, but it doesn’t trivially allow two different files to be diffed. So to demonstrate how diffing works, I've pasted `bendall-cv-sanitized.txt` and `ms-kd14--kd15-santized.txt` as two different versions of `diff-bendall-ms.txt`. [You can view the diff here](https://github.com/sujato/bendall-cv/commit/b578fbf3549291ef839fae2711b43790b9fe55ef).

It doesn't work 100%, as Github doesn't represent all the diffs properly, but it's good enough to see the concept.
