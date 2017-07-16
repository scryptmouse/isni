A small class for generating and validating Internation Standard Name
Identifiers (ISNI). This will also work just fine with ORCID, a subset
of ISNI.

# Installation

    gem install isni

# Usage

    ISNI.new("000000029534656X").valid?
    => true

    ISNI.valid?("000000029534656X")
    => true

    ISNI.valid?("0000000295346560")
    => false

    ISNI.complete("000000029534656")
    => "000000029534656X"

    ISNI.new("000000029534656X").to_s
    => "0000-0002-9534-656X"

# Further Reading

- http://en.wikipedia.org/wiki/International_Standard_Name_Identifier
- http://orcid.org/
- http://support.orcid.org/knowledgebase/articles/116780-structure-of-the-orcid-identifier

# Contributing

Source code is publicly available @ http://github.com/yob/isni. Patches
welcome, preferably via a git repo I can pull from.
