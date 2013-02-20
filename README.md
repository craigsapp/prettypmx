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


