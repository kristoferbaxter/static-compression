Why use Brotli and Zopfli?
--------------------------

Brotli and Zopfli offer significant compression advantages over gzip. Here are some small examples.

Twitter for me appears to have five main bundles (when visiting on a desktop machine).
1. init.en.b42e0a665272da1c4fde.js
    live - 195230
    gzip (9) - 193248, 1% less
		zopfli (i1000) - 183433, 6.04% less
		brotli (q11) - 156856, 19.6% less
2. 17.commons.en.9afdd1690c7f944c1647.js
    live - 134220
    gzip (9) - 130627, 2.67% less
		zopfli (i1000) - 125897, 6.20% less
		brotli (q11) - 106251, 20.8% less
3. 7.pages_home.en.8ab8ff706989bc27ef69.js
    live - 66138
		gzip (9) - 64445, 2.56% less
		zopfli (i1000) - 62122, 6.07% less
		brotli (q11) - 55538, 16% less
4. analytics.js
    live - 12156
		gzip (9) - 12169, worse!
		zopfli (i1000) - 11777, 3.11% less
		brotli (q11) - 10839, 10.8% less
5. native_bundle_v1_5e8d344810971de9481b549eea8788580bef3484.js
    live - 38889
		gzip (9) - 38308, 1.49% less
		zopfli (i1000) - 37078, 4.65% less
		brotli (q11) - 33162, 14.7% less