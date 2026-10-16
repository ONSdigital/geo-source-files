# Geography source files

An archive of the source files used by [ONSdigital/geo-scripts](https://github.com/ONSdigital/geo-scripts), which generates geographic data for ONS Data Visualisation products.

The files are downloaded from the [ONS Open Geography Portal](https://geoportal.statistics.gov.uk) and other sources, and kept here so they stay available after datasets are retired or replaced. They are stored as **release assets**, not in the repository itself; see [Releases](https://github.com/ONSdigital/geo-source-files/releases).

- Each geography and year has its own release, tagged `{key}-{year}` (eg. `wd-2025`). It holds that year's boundary files as gzipped GeoJSONSeq (eg. `wd25_bfc.json.gz`, one feature per line).
- The `other` release holds other source files, such as lookups and the NSPL.
- Each release has a `manifest.json`, listing every file's source dataset, SHA-256 checksum and the date it was archived.

There is one version of each file: corrected files replace the previous version under the same tag.

The files are managed by the `download-files` and `archive-sources` scripts in geo-scripts; see [its documentation](https://github.com/ONSdigital/geo-scripts/blob/main/docs/Source-file-archive.md).

Source data: Office for National Statistics, licensed under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/). Contains OS data © Crown copyright and database right.
