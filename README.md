# DH Journals List

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)

**View the interactive list:** https://dhjournals.github.io/list/

## Overview

This repository contains a comprehensive list of **Digital Humanities journals** that have been retrieved through automatic extraction and manual curation. The list includes journals at different levels of Digital Humanities focus:

- **Exclusively**: Journals completely devoted to publishing Digital Humanities articles
- **Significantly**: Journals where a significant set of publications deal with Digital Humanities
- **Marginally**: Journals where only a small set of publications are Digital Humanities
- **Mega-journal**: Large multidisciplinary journals that may include some DH content

## Main Resources

### Journal List Website
The interactive, searchable journal list is available at: **https://dhjournals.github.io/list/**

The website features:
- Dynamic loading from TSV data
- Sortable and filterable table
- Color-coded DH level indicators
- Direct links to journal websites

### Citations & Research

The list has been developed and used in the following publications:

- **Spinaci, G., Colavizza, G., and Peroni, S.** (2020). Preliminary results on mapping digital humanities Research, Proceedings of L'Associazione per l'Informatica Umanistica e La Cultura Digitale, pp. 246–252. [PDF](https://aiucd2020.unicatt.it/aiucd-Spinaci_et_al.pdf)

- **Spinaci, G., Colavizza, G., and Peroni, S.** (2022). A map of Digital Humanities research across bibliographic data sources, Digital Scholarship in the Humanities. [DOI: 10.1093/llc/fqac016](https://doi.org/10.1093/llc/fqac016)

**Note:** The citation analysis and network data covers journals through iteration 3. Journals added in iteration 4 and beyond are not included in the citation analysis.

### Data Download
The complete dataset is available on Zenodo: https://zenodo.org/record/3406564

## Repository Structure

### `data/`
The data directory contains the journal list and citation analysis results:

- **`dhjournals.tsv`**: Main journal list with metadata (ID, E-ISSN, P-ISSN, Title, URL, DH Level, Iteration)

#### `data/citations/`
Citation analysis data from multiple bibliographic sources:

- **`crossref/`**: Citation distributions from Crossref
- **`dimensions/`**: Citation distributions from Dimensions
- **`msacademic/`**: Citation distributions from Microsoft Academic
- **`scopus/`**: Citation distributions from Scopus
- **`wos/`**: Citation distributions from Web of Science

Each source contains:
- `data/`: TSV files with incoming/outgoing citation distributions
- `pics/`: Visualization charts of citation patterns

#### `data/clusters/`
VOSViewer network analysis maps for each bibliographic source:

- `dimensions/VOSViewer_DIMENSIONS_map.txt`
- `msacademic/VOSViewer_MAG_map.txt`
- `scopus/VOSViewer_SCOPUS_map.txt`
- `wos/VOSViewer_WOS_map.txt`

#### `data/publications/`
Publication-level analysis data:

- `cluster_frequent_terms.tsv`: Most frequent terms in publication clusters
- `pubs_level.tsv`: Publication counts by DH level

Available for: Crossref, Dimensions, Microsoft Academic, Scopus, and Web of Science

## Contributing

### Adding a Journal

To suggest a new journal for the list:

1. Go to [Issues](https://github.com/dhjournals/list/issues)
2. Click "New Issue"
3. Select "Add Journal"
4. Fill in the journal information

New journals will be reviewed and added to the appropriate iteration.

### Updating the List

The journal list is maintained in `data/dhjournals.tsv`. Updates to this file will automatically reflect on the website.

## License

This work is licensed under [CC0 1.0 Universal (CC0 1.0) Public Domain Dedication](http://creativecommons.org/publicdomain/zero/1.0/).
