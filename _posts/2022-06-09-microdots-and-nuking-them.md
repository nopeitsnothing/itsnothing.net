---
layout: post
title: Removing microdots from printed documents
---

Anonymize your documents by removing metadata and ensure you don't have any
identifying marks embedded.

For hundreds of years, paper and printing techniques are the foundation for
distribution of information. Thereby, physical documents enjoy high
confidence. To have something in "black and white" carries significance. But
forgery or alteration of documents are nearly as old as the history of
writing. Hence the question for the originator is important. Nowadays,
because of continual technological development, even individuals can print
high-quality documents and duplicates. This can be done with cheap and
customary devices. In addition image processing software, like GIMP or Adobe
Photoshop, allows to manipulate documents and images easily. Therefore
printed documents are often an issue in crimes, e.g. faked proof of identity,
copyright theft, or as exhibit in a criminal case. In all this cases it could
be useful for law enforcement agencies to, e.g., identify the device or model
which was used to print the questionable document.

The primary focus of the research lies on the extraction of artifacts, which
are originated from the print process. These artifacts emerge particularly
through electromechanical imperfections and also through differences between
constructions of printer models. We try to find and analyze artifacts which
are stable and e.g. model specific and therefore usable as intrinsic
signatures for a specific printer model. The extraction of these signatures
should be conducted with customary scanner devices and image processing
techniques. Simultaneously, the company Dence (cooperation partner) will
investigate the scanner forensics.

The second part of the project deals with research of print-scan resilient
checks of duplicates. Here the knowledge about artifacts which occur in the
print and scan process represent a reliable basis. As use case the typical
workflow in an insurance can be mentioned. In the event of damage, the
insured person would take a photo of the damage and send it postal, together
with forms, to the insurance. Afterwards the insurance will scan these
documents. The insurance staff examines the event of damage on the basis of
the digital reproduction. Because of the print and scan processes, which the
original document went through, the question of authenticity of the document
is difficulty to answer. Goal of the analysis is the implementation of an
image search for duplicates, which is resilient against the print and scan
process. This means, that images can also be matched, if only printed and
re-digitized versions are available. The duplicate testing must be able to
check an image immediately against a data pool with millions of images. From
technical view, this will be realized with a distinct image hash. The
challenge for the print-scan scenario is the computation of this hash. The
hash value has to be equal or very similar between the original photo and the
printed and re-digitized image, so that they can matched. Another difficulty
is a working check for duplicates also with slight manipulations in the
image (like a car scratch). All of this must be accomplished without matching
false positives.

### References
* https://dfd.inf.tu-dresden.de/
* https://github.com/dfd-tud/deda
