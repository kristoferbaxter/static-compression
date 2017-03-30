Why use Brotli and Zopfli?
--------------------------

Brotli and Zopfli offer significant compression advantages over gzip. Here are some small examples.

Twitter for me appears to have five main bundles (when visiting on a desktop machine).

| File                        | live   | gzip 9         | zopfli (i1000) | brotli (q11)   |
| --------------------------- |:------:| --------------:| --------------:| --------------:|
| init.en.{hash}.js           | 195230 | 193248 (1%)    | 183433 (6.04%) | 156856 (19.6%) |
| 17.commons.en.{hash}.js     | 134220 | 130627 (2.67%) | 125897 (6.2%)  | 106251 (20.8%) |
| 7.pages_home.en.{hash}.js   | 66138  | 64445 (2.56%)  | 62122 (6.07%) | 55538 (16%)    |
| analytics.js                | 12156  | 12169 (worse!) | 11777 (3.11%)  | 10839 (10.8%)  |
| native_bundle_v1_{hash}.js  | 38889  | 38308 (1.49%)  | 37078 (4.65%)  | 33162 (14.7%)  |
