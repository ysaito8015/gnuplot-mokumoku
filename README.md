## install gnuplot

```sh
$ sudo apt install gnuplot
```

## start

```sh
$ gnuplot
```


```
gnuplot> plot './data/2col.data'
```


- Assumes col12 = x, col2 = y
- Shows '+' at data points
- Does not connect ponts with a line
- Opens plot in a 'qt window'


### Variations
```
gnuplot> plot './data/2col.data'
gnuplot> plot './data/2col.data' with lines
gnuplot> plot './data/2col.data' with linespoints
gnuplot> plot './data/2col.data' with points
gnuplot> plot[1:5] './data/2col.data' with points
gnuplot> plot[3:7] './data/2col.data' with points
gnuplot> plot './data/2col.data' with lines title 'my curve'
gnuplot> plot './data/2col.data' using 1:2 with linespoints
gnuplot> plot './data/2col.data' using 2:1 with linespoints
gnuplot> plot './data/2col.data' using 1:2 with linespoints title 'Squared'
gnuplot> plot './data/2col.data' u 1:2 w lp title 'Squared'
```


### Outputs

```
gnuplot> set terminal png
gnuplot> set output './outputs/01.png'
gnuplot> plot './data/2col.data' u 1:2 w lp title 'Squared'
```
