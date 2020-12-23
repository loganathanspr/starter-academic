---
title: Wikipedia Spelling Error Corpus
summary: Scripts for extracting spelling errors from Wikipedia revisions
tags:
- ETL
- Datasets
- Wikipedia
date: "2015-12-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/ufal/wiki-error-corpus"

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/ufal/wiki-error-corpus
url_code: ""
url_project: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

{{% callout note %}}
This page contains only minimal description of the project. More detailed documentation is available at http://ufal.mff.cuni.cz/~ramasamy/tamiltb/0.1/
{{% /callout %}}

Tamil Dependency Treebank version 0.1 (TamilTB.v0.1) is an attempt to develop a syntactically annotated corpora for Tamil. TamilTB.v0.1 contains 600 sentences enriched with manual annotation of morphology and dependency syntax in the style of Prague Dependency Treebank. TamilTB.v0.1 has been created at the Institute of Formal and Applied Linguistics, Charles University in Prague.

Treebank is an important resource in building parsers and analyzing the language. As far as our knowledge is concerned, this is the first attempt to build a treebank for Tamil language. Tamil belongs to Dravidian family of languages and mainly spoken in Southern part of India. Main features of the Tamil language include Subject-Object-Verb (SOV) word order, morphologically rich and agglutination.

The main objectives of this project include,
<ol>
<li>Annotate data at word level and syntactic level</li>
<li>In each level of annotation, trying for maximum level of linguistic representation</li>
<li>Building large annotated corpora using automatic annotation process.</li>
</ol>

The data used for the TamilTB annotation comes from the news domain. We decided to use the news data for  two reasons: (i) huge amount of data is available in digital format and can be easily downloadable and (ii) the news data can be considered as representative of written Tamil. At present, the data for the annotation comes from  www.dinamani.com , and we downloaded pages randomly covering various news topics. The table below summarises the data used for annotation.

| No | Description                          | Value |
| -- | ------------------------------------ | ----- |
| 1  | Source                               | www.dinamani.com |
| 2  | Source transliterated                | Yes   |
| 3  | Number of Words                      | 9581  |
| 4  | Number of Sentences                  | 600   |
| 5  | Morphological Layer Annotation (sen) | 600   |
| 6  | Syntactic Annotation (sen)           | 600   |
| 7  | Tectogrammatical Layer Annotation    | -   |


## Download TamilTB.v0.1
The single package containing the data and the documentation can be downloaded from the following link,

http://ufal.mff.cuni.cz/~ramasamy/tamiltb/0.1/TamilTB.v0.1.tar.gz

The package can be uncompressed using the following command,

```
[shell]$ tar -zxvf TamilTB.v0.1.tar.gz
```

### Contents of TamilTB.v0.1.tar.gz

```
- TamilTB.v0.1/ (top level directory)
      - data/
           TamilTB.v0.1.tmt (in TMT format)
           TamilTB.v0.1.conll (in CoNLL format, transliterated)
           TamilTB.v0.1.utf8.conll (in CoNLL format, UTF8)
           TamilTB.v0.1.tt (only POS tagged corpora in TnT style, transliterated)
           TamilTB.v0.1.utf8.tt (only POS tagged corpora in TnT style, UTF8)
      - doc/
           index.html (main page)
           ...
           ...
           ...
      - README.txt
````


### Prerequisites

The annotated data in TMT format requires TrEd to be installed. TrEd can be downloaded from  http://ufal.mff.cuni.cz/~pajas/tred/

After installing TrEd, you need to install TMT plugin to browse the treebank data in the tmt file. The plugin can be installed by following

```
Setup -> Manage Extensions -> "TMT files support" in the TrEd.
```

Then treebank can be browsed by opening TamilTB.v0.1.tmt in TrEd.
