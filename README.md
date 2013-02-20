The _prettypmx_ PERL script aligns parameter matrices of SCORE PMX
data.  Trailing zeros in fractional portations are adjusted so that
each column contains the same number of fractional digits (for
readability and compactness).

Example input:

<pre>
8.  1.0    .000      .00      .60   41.70
3.  1.0   1.200      .00     1.00
18.  1.0   5.700      .00    99.00     1.00
1.  1.0  11.640     8.00    20.00      .00     1.0000
1.  1.0  11.640    12.00    10.00      .00     1.0000    -1.50
14.  1.0  15.788     2.00
1.  1.0  17.618    11.00    20.00      .00     1.0000
1.  1.0  17.620    11.00    10.00      .00      .5000    -1.00      .00
6.  1.0  17.620    10.00     9.00    21.76    11.0000
1.  1.0  21.758    10.00    12.00      .00      .5000    -1.00      .00
1.  1.0  25.897     4.00    20.00      .00     1.0000    -1.50
1.  1.0  25.900     9.00    12.00      .00     1.0000    -1.00
1.  1.0  33.027     8.00    20.00      .00     1.0000      .00      .00      .00   -14.00
1.  1.0  33.028    10.00    10.00      .00     1.0000    -1.50
1.  1.0  37.552     7.00    20.00      .00     1.0000
1.  1.0  37.553    12.00    10.00      .00     1.0000    -1.50
14.  1.0  41.700     2.00
</pre>

Example output:

<pre>
8  1  0.000  0  0.6 41.70
3  1  1.200  0  1.0
18 1  5.700  0 99.0  1.00
1  1 11.640  8 20.0  0.00  1.0
1  1 11.640 12 10.0  0.00  1.0 -1.5
14 1 15.788 
1  1 17.618 11 20.0  0.00  1.0
1  1 17.620 11 10.0  0.00  0.5 -1.0
6  1 17.620 10  9.0 21.76 11.0
1  1 21.758 10 12.0  0.00  0.5 -1.0
1  1 25.897  4 20.0  0.00  1.0 -1.5
1  1 25.900  9 12.0  0.00  1.0 -1.0
1  1 33.027  8 20.0  0.00  1.0  0.0 0 0 -14
1  1 33.028 10 10.0  0.00  1.0 -1.5
1  1 37.552  7 20.0  0.00  1.0
1  1 37.553 12 10.0  0.00  1.0 -1.5
14 1 41.700
</pre>

Both the example input and output PMX data will produce this image in the SCORE editor:

<center>
   <img type="image/svg+xml" src="example/example.svg?raw=true">
</center>

<center>
   <img type="image/svg+xml" src="http://htmlpreview.github.com/?http://raw.github.com/craigsapp/prettypmx/master/example/example.svg">
</center>

<center>
   <object type="image/svg+xml" data="http://htmlpreview.github.com/?http://raw.github.com/craigsapp/prettypmx/master/example/example.svg">
</object>
</center>

<center>
   <embed type="image/svg+xml" src="http://htmlpreview.github.com/?http://raw.github.com/craigsapp/prettypmx/master/example/example.svg">
</center>

<center>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN"
  "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<svg version="1.1"
     xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     viewBox="37 0 114 38"
     width="342" height="114">
<g transform="translate(0,86) scale(1,-1) scale(.01800) translate(2100,27250)" stroke-linejoin="round" color="black" stroke="currentColor" fill="none" stroke-width="26.7067"  fill-rule="evenodd">
<defs>
<g id="P00">
<path  d="
M118 -168
L162 -168
L200 -162
L256 -143
L306 -118
L350 -87
L368 -68
L400 -31
L418 6
L425 43
L425 68
L418 93
L412 106
L393 131
L368 150
L356 156
L337 162
L306 168
L262 168
L225 162
L187 150
L168 143
L118 118
L75 87
L56 68
L25 31
L6 -6
L0 -43
L0 -68
L6 -93
L12 -106
L31 -131
L56 -150
L68 -156
L87 -162
L118 -168
Z" fill="currentColor"/>
</g>
</defs>
<defs>
<g id="P01">
<path  d="
M-356 400
L-356 -425
M-218 -375
L-218 450
"/>
<path  d="
M-125 212
L-125 262
L-450 162
L-450 81
L-125 181
L-125 212
Z" fill="currentColor"/>
<path  d="
M-125 -93
L-125 -56
L-450 -156
L-450 -237
L-125 -137
L-125 -93
Z" fill="currentColor"/>
</g>
</defs>
<path stroke-width="20.0300" d="
M0 -24000
L6255 -24000
M0 -23790
L6255 -23790
M0 -23580
L6255 -23580
M0 -23370
L6255 -23370
M0 -23160
L6255 -23160
"/>
<path  d="
M180 -23381
L187 -23400
L198 -23415
L213 -23430
L232 -23437
L255 -23441
L262 -23441
L288 -23437
L307 -23430
L322 -23418
L333 -23403
L341 -23388
L345 -23366
L345 -23355
L341 -23336
L333 -23321
L318 -23306
L307 -23298
L292 -23291
L273 -23287
L255 -23287
L232 -23295
L221 -23302
L210 -23321
L198 -23310
L202 -23283
L210 -23261
L217 -23246
L236 -23216
L213 -23238
L202 -23253
L195 -23268
L183 -23298
L176 -23328
L176 -23351
L180 -23381
Z" fill="currentColor"/>
<path  d="
M236 -23216
L262 -23197
L285 -23186
L307 -23178
L330 -23175
"/>
<path  d="
M277 -23782
L322 -23756
L375 -23722
L431 -23677
L480 -23628
L502 -23598
L528 -23561
L543 -23531
L558 -23497
L566 -23471
L570 -23445
L573 -23411
L573 -23385
L570 -23347
L562 -23321
L551 -23291
L540 -23268
L521 -23242
L502 -23223
L480 -23208
L465 -23197
L438 -23186
L412 -23178
L378 -23175
L330 -23175
L375 -23182
L393 -23190
L416 -23205
L438 -23231
L450 -23250
L461 -23280
L468 -23317
L472 -23362
L472 -23403
L468 -23463
L461 -23505
L453 -23538
L442 -23576
L423 -23617
L408 -23643
L386 -23673
L360 -23703
L345 -23718
L318 -23741
L288 -23763
L266 -23778
L221 -23805
L150 -23842
L150 -23846
L198 -23823
L277 -23782
Z" fill="currentColor"/>
<path  d="
M633 -23272
L637 -23280
L645 -23291
L656 -23295
L667 -23295
L678 -23291
L686 -23280
L690 -23272
L690 -23257
L686 -23250
L678 -23238
L667 -23235
L656 -23235
L645 -23238
L637 -23250
L633 -23257
L633 -23272
Z" fill="currentColor"/>
<path  d="
M633 -23478
L637 -23486
L645 -23497
L656 -23501
L667 -23501
L678 -23497
L686 -23486
L690 -23478
L690 -23463
L686 -23456
L678 -23445
L667 -23441
L656 -23441
L645 -23445
L637 -23456
L633 -23463
L633 -23478
Z" fill="currentColor"/>
<path  d="
M1226 -23651
L1226 -23685
L1215 -23718
L1181 -23752
L1147 -23775
L1091 -23786
L1057 -23786
M1068 -23381
L1102 -23381
L1158 -23392
L1181 -23403
L1215 -23437
L1226 -23482
L1226 -23505
"/>
<path  d="
M1080 -23786
L1035 -23786
L978 -23775
L933 -23752
L911 -23730
L888 -23696
L877 -23673
L866 -23617
L866 -23561
L877 -23493
L900 -23448
L933 -23415
L967 -23392
L1023 -23381
L1080 -23381
L1012 -23392
L978 -23415
L967 -23437
L956 -23482
L956 -23685
L967 -23730
L978 -23752
L1012 -23775
L1080 -23786
Z" fill="currentColor"/>
<path  d="
M1226 -23516
L1215 -23538
L1203 -23550
L1181 -23561
L1147 -23561
L1125 -23550
L1113 -23538
L1102 -23516
L1102 -23482
L1113 -23460
L1125 -23448
L1147 -23437
L1181 -23437
L1203 -23448
L1215 -23460
L1226 -23482
L1226 -23516
Z" fill="currentColor"/>
<use transform="translate(1746,-23475) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M1746 -23506
L1746 -24210
"/>
<use transform="translate(1746,-23055) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M2001 -23023
L2001 -22477
"/>
<path  d="
M2368 -24000
L2368 -23160
M2374 -24000
L2374 -23160
"/>
<use transform="translate(2642,-23160) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M2642 -23191
L2642 -23895
"/>
<use transform="translate(2643,-23160) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M2898 -23128
L2898 -22530
"/>
<path stroke-width=".0000" d="
M3519 -22740
L3519 -22635
L2898 -22530
L2898 -22635
L3519 -22740
L3519 -22635
Z" fill="currentColor"/>
<use transform="translate(3263,-23265) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<use transform="translate(3263,-23265) scale(.600)" stroke-width="44.511" xlink:href="#P01"/>
<path  d="
M3518 -23233
L3518 -22635
"/>
<use transform="translate(3884,-23895) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M3884 -23926
L3884 -24472
"/>
<use transform="translate(3885,-23370) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<use transform="translate(3885,-23370) scale(.600)" stroke-width="44.511" xlink:href="#P01"/>
<path  d="
M4140 -23338
L4140 -22740
"/>
<use transform="translate(4954,-23475) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M4954 -23506
L4954 -24210
"/>
<path  d="
M5272 -24330
L5265 -24371
L5254 -24412
L5242 -24442
L5231 -24465
L5216 -24487
L5197 -24506
L5171 -24521
L5149 -24528
L5122 -24532
L5089 -24532
L5062 -24528
L5040 -24521
L5014 -24506
L4995 -24487
L4980 -24465
L4969 -24442
L4957 -24412
L4946 -24371
L4939 -24330
L4965 -24390
L4976 -24412
L4984 -24423
L4999 -24442
L5021 -24461
L5036 -24468
L5047 -24472
L5059 -24476
L5081 -24480
L5130 -24480
L5152 -24476
L5164 -24472
L5175 -24468
L5190 -24461
L5212 -24442
L5227 -24423
L5235 -24412
L5246 -24390
L5272 -24330
Z" fill="currentColor"/>
<path  d="
M5137 -24378
L5130 -24393
L5115 -24401
L5096 -24401
L5081 -24393
L5074 -24378
L5074 -24360
L5081 -24348
L5096 -24341
L5115 -24341
L5130 -24348
L5137 -24360
L5137 -24378
Z" fill="currentColor"/>
<use transform="translate(4954,-23265) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M5209 -23233
L5209 -22687
"/>
<use transform="translate(5632,-23580) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M5632 -23611
L5632 -24315
"/>
<use transform="translate(5632,-23055) scale(.600)" stroke-width="44.511" xlink:href="#P00"/>
<path  d="
M5887 -23023
L5887 -22477
"/>
<path  d="
M6255 -24000
L6255 -23160
M6261 -24000
L6261 -23160
"/>
</g>
</svg>
<?SCORE version="4"
#SVG_SCALE: 3
8  1  0.000  0  0.6 41.70
3  1  1.200  0  1.0
18 1  5.700  0 99.0   1.00
1  1 11.640  8 20.0   0.00  1.0
1  1 11.640 12 10.0   0.00  1.0 -1.5
14 1 15.788
1  1 17.618 11 20.0   0.00  1.0
1  1 17.620 11 10.0   0.00  0.5 -1.0
6  1 17.620 10  9.0  21.76 11.0
1  1 21.758 10 12.0   0.00  0.5 -1.0
1  1 25.897  4 20.0   0.00  1.0 -1.5
1  1 25.900  9 12.0   0.00  1.0 -1.0
1  1 33.027  8 20.0   0.00  1.0  0.0 0 0 -14
1  1 33.028 10 10.0   0.00  1.0 -1.5
1  1 37.552  7 20.0   0.00  1.0
1  1 37.553 12 10.0   0.00  1.0 -1.5
14 1 41.700
?>
</center>

