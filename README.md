# aj-wrangle
## Alekhya Jaddu - In person class bonus challenge
## Play URL
Comedy Number 6

Measure for Measure

http://shakespeare.mit.edu/measure/full.html

## Speakers
1. DUKE VINCENTIO
2. ISABELLA

## Question
To compare the number of times each speaker, spoke during the play.

## Commands Used
```
curl "http://shakespeare.mit.edu/measure/full.html" -O "data.txt"
curl "http://shakespeare.mit.edu/measure/full.html" | sed 's/<\/*[^>]*>//g' > data.txt
grep 'DUKE VINCENTIO' data.txt -c
grep 'ISABELLA' data.txt -c
grep 'DUKE VINCENTIO' data.txt -c > result-duke.txt
grep 'ISABELLA' data.txt -c > result-isabella.txt
```

## Result
- 'DUKE VINCENTIO' spoke for about 207 times where as 'ISABELLA' spoke for 156 times.
- 'DUKE VINCENTIO' speaks more than 'ISABELLA'.

## Input file
[data.txt](https://github.com/alekhyajaddu/aj-wrangle/blob/main/data.txt)

## Output file
[result-duke](https://github.com/alekhyajaddu/aj-wrangle/blob/main/result-duke.txt)

[result-isabella](https://github.com/alekhyajaddu/aj-wrangle/blob/main/result-isabella.txt)




