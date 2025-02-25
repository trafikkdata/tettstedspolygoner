# Administrative area polygons
This repo contains releases with administrative area files.

There should be 1 release per year that we need.

## 📜 Uploading a New Dataset
A new dataset is released every year with a one-year delay, i.e., in 2025 the dataset for 2024 becomes available.

1) Download the latest dataset from [Geonorge](https://kartkatalog.geonorge.no/metadata/tettsteder/173f4a15-dead-4f82-b92e-f37396b72cea).
2) Create a release in this repository, [https://github.com/trafikkdata/tettstedspolygoner/releases](https://github.com/trafikkdata/tettstedspolygoner/releases)
3) Use the Traffic-Link endpoint `POST /urban-area/upload-urban-areas-from-remote-file` in OPS. Set `externalLink` to the link to download the dataset from your release. For example, for 2024, `externalLink` was `https://github.com/trafikkdata/tettstedspolygoner/releases/download/2024/Befolkning_0000_Norge_25833_Tettsteder2024_GML.gml`.
4) Verify that an index called `urban_area_polygon_[YOUR CHOSEN YEAR]`appears in ES Analysis.