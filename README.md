# Google scholar entry collector

A Python script that collect publication information from google scholar. It uses 
the the scholarly library.

To use it, replace the `scholar_url` in `collect_publications.py` with your
scholar URL, and run `collect_publications.py` with Python:

```bash
    python3 collect_publications.py
```

By default, publication information is written in a folder YEAR_NAME_JOURNAL,
located in `path`, to a file named `index.md` that can be read with Hugo webpage,
just like [this one](https://simongravelle.github.io).

Output looks like that:
```bash
---
title: "Optimizing water permeability through the hourglass shape of aquaporins"
date: 2013-09-25
publishDate: 2013-09-25
authors: ["**Simon Gravelle**", "Laurent Joly", "François Detcheverry", "Christophe Ybert", "Cécile Cottin-Bizonne", "Lydéric Bocquet"]
publication_types: ["2"]
abstract: "Aquaporin channels are able to selectively conduct water across cell membranes, with remarkable efficiency. Although molecular details are crucial to the pore performance, permeability is also strongly limited by viscous dissipation at the entrances. Could the hourglass shape of aquaporins optimize such entrance effects? We show that conical entrances with suitable opening angle can indeed provide a large increase of the channel permeability. Strikingly, the optimal opening angles compare well with the angles measured in a large variety of aquaporins, suggesting that their hourglass shape could be the result of a natural selection process toward optimal permeability. This work also provides guidelines to optimize the performances of artificial nanopores, with applications in desalination, ultrafiltration, or energy conversion."
featured: true
publication: "Proceedings of the National Academy of Sciences, 110, 41"
links:
  - icon_pack: fas
    icon: scroll
    name: Link
    url: 'https://doi.org/10.1073/pnas.1306447110'
---
```