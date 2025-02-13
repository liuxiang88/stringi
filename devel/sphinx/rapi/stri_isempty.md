# stri\_isempty: Determine if a String is of Length Zero

## Description

This is the fastest way to find out whether the elements of a character vector are empty strings.

## Usage

```r
stri_isempty(str)
```

## Arguments

|       |                                            |
|-------|--------------------------------------------|
| `str` | character vector or an object coercible to |

## Details

Missing values are handled properly.

## Value

Returns a logical vector of the same length as `str`.

## Author(s)

[Marek Gagolewski](https://www.gagolewski.com/) and other contributors

## See Also

The official online manual of <span class="pkg">stringi</span> at <https://stringi.gagolewski.com/>

Other length: [`%s$%()`](+25s+24+25.md), [`stri_length()`](stri_length.md), [`stri_numbytes()`](stri_numbytes.md), [`stri_pad_both()`](stri_pad.md), [`stri_sprintf()`](stri_sprintf.md), [`stri_width()`](stri_width.md)

## Examples




```r
stri_isempty(letters[1:3])
## [1] FALSE FALSE FALSE
stri_isempty(c(',', '', 'abc', '123', '\u0105\u0104'))
## [1] FALSE  TRUE FALSE FALSE FALSE
stri_isempty(character(1))
## [1] TRUE
```
