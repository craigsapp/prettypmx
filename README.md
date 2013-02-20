The _prettypmx_ PERL script aligns parameter matrices of SCORE PMX
data.  Trailing zeros in fractional portions of numbers are adjusted
so that each column contains the same number of fractional digits
(for readability and compactness).

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

Both the example input and output PMX data will produce this image in the SCORE editor (loaded with the REad command):

<center>
![Example notation](example/example.png?raw=true)
</center>

The _prettypmx_ program accepts one option (-s) which can change
the spacing between columns to something other than a single space.
Here is an example placing three spaces between columns:

<pre>prettypmx -s "   " input.pmx > output2.pmx</pre>

<pre>
8    1    0.000    0    0.6   41.70
3    1    1.200    0    1.0
18   1    5.700    0   99.0    1.00
1    1   11.640    8   20.0    0.00    1.0
1    1   11.640   12   10.0    0.00    1.0   -1.5
14   1   15.788    2
1    1   17.618   11   20.0    0.00    1.0
1    1   17.620   11   10.0    0.00    0.5   -1.0
6    1   17.620   10    9.0   21.76   11.0
1    1   21.758   10   12.0    0.00    0.5   -1.0
1    1   25.897    4   20.0    0.00    1.0   -1.5
1    1   25.900    9   12.0    0.00    1.0   -1.0
1    1   33.027    8   20.0    0.00    1.0    0.0   0   0   -14
1    1   33.028   10   10.0    0.00    1.0   -1.5
1    1   37.552    7   20.0    0.00    1.0
1    1   37.553   12   10.0    0.00    1.0   -1.5
14   1   41.700    2
</pre>

Text for code 16 items will not be altered.  For example, below is output 
from prettypmx which adds two spaces between columns.  Note that the text
"Allegro ma non troppo" retains single space between the words.

<pre>
8   6  20.000   6.270   0.8
3   6  22.333
17  6  29.267   0.000   5.0
18  6  41.528   0.000  99.0   1.000
t   6  42.505  13.625   1.0   1.291   0.00   0.00  0  0.0  -1.08
_00Allegro ma non troppo
2   6  51.228   0.000   0.0   0.000   1.00
9   6  69.034  13.000  53.0   1.000
1   6  69.034   2.000  10.0   0.000   0.25   3.50
6   6  69.034   5.500   8.0  82.390  12.00
1   6  69.034   2.000  20.0   0.000   1.00  -1.50
5   6  70.284   0.540   6.0  83.260  -2.00  -1.00  0  0.6   0.00  0  0.5
1   6  73.485   7.000  10.0   0.000   0.25  -0.67
1   6  77.937   4.000  10.0   0.000   0.25   3.17
1   6  82.388   9.000  10.0   0.000   0.25  -1.00
2   6  86.840   0.000   0.0   0.000   1.00
</pre>


