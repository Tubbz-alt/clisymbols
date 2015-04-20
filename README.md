



# prettysymbols

> Unicode symbols with Windows fallbacks

![](screenshot.png)

## Install


```r
install.packages("devtools")
devtools::install_github("gaborcsardi/prettysymbols")
```

## Usage


```r
library(prettysymbols)
cat(symbol$check, "All good\n")
```

```
#>  All good
```

```r
cat(symbol$cross, "Problem\n")
```

```
#> ✖ Problem
```

Here is a list of all symbols, with their names:


```r
for (i in seq_along(symbol)) {
  cat(symbol[[i]], "\t", names(symbol)[i], "\n")
}
```

```
#> ✔ 	 tick 
#> ✖ 	 cross 
#> ★ 	 star 
#> ▇ 	 square 
#> ◻ 	 square_small 
#> ◼ 	 square_small_filled 
#> ◯ 	 circle 
#> ◉ 	 circle_filled 
#> ◌ 	 circle_dotted 
#> ◎ 	 circle_double 
#> ⓞ 	 circle_circle 
#> ⓧ 	 circle_cross 
#> Ⓘ 	 circle_pipe 
#> ?⃝ 	 circle_question_mark 
#> ● 	 bullet 
#> ․ 	 dot 
#> ─ 	 line 
#> … 	 ellipsis 
#> ❯ 	 pointer 
#> ℹ 	 info 
#> ⚠ 	 warning 
#> ☰ 	 menu 
#> ☺ 	 smiley 
#> ෴ 	 mustache 
#> ♥ 	 heart 
#> ↑ 	 arrow_up 
#> ↓ 	 arrow_down 
#> ← 	 arrow_left 
#> → 	 arrow_right 
#> ◉ 	 radio_on 
#> ◯ 	 radio_off 
#> ☒ 	 checkbox_on 
#> ☐ 	 checkbox_off 
#> ⓧ 	 checkbox_circle_on 
#> Ⓘ 	 checkbox_circle_off
```

### Fallback symbols

Some terminals do not support (all) Unicode characters, and on these reasonable
ASCII substitutes are used:


```
#> √ 	 tick 
#> x 	 cross 
#> * 	 star 
#> █ 	 square 
#> [ ] 	 square_small 
#> [█] 	 square_small_filled 
#> ( ) 	 circle 
#> (*) 	 circle_filled 
#> ( ) 	 circle_dotted 
#> (o) 	 circle_double 
#> (o) 	 circle_circle 
#> (x) 	 circle_cross 
#> (|) 	 circle_pipe 
#> (?) 	 circle_question_mark 
#> * 	 bullet 
#> . 	 dot 
#> ─ 	 line 
#> ... 	 ellipsis 
#> > 	 pointer 
#> i 	 info 
#> ‼ 	 warning 
#> ≡ 	 menu 
#> ☺ 	 smiley 
#> ┌─┐ 	 mustache 
#>  	 heart 
#> ^ 	 arrow_up 
#> v 	 arrow_down 
#> < 	 arrow_left 
#> > 	 arrow_right 
#> (*) 	 radio_on 
#> ( ) 	 radio_off 
#> [x] 	 checkbox_on 
#> [ ] 	 checkbox_off 
#> (x) 	 checkbox_circle_on 
#> ( ) 	 checkbox_circle_off
```

# License

MIT © [Gabor Csardi](http://gaborcsardi.org) and [Sindre Sorhus](http://sindresorhus.com)
