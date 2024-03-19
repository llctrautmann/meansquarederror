+++
title = 'Encodings'
date = 2024-03-11T16:39:38+01:00
draft = false
mathjax = true
+++

### Text Input

$$\text{{text}} = \text{"Tokens in NLP."}$$

### Tokenised Letters

$$[\text{T}, \text{o},\text{k},\text{e},\text{n},\text{s},\text{ },\text{i},\text{n}, \text{ }, \text{N},\text{L}, \text{P}, \text{.}]$$

### Index Encoding Scheme

$$[\text{' '}: 0, \text{.}: 1, \text{L}: 2, \text{N}: 3, \text{P}: 4, \text{T}: 5,\text{e}: 6, \text{i}: 7, \text{k}: 8, \text{n}: 9, \text{o}: 10, \text{s}: 11]$$

### Encoded Text

$$[5, 10, 8, 6, 9, 11, 0, 7, 9, 0, 3, 2, 4, 1]$$

### One Hot Encoding

| word | token | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | 10  | 11  | 12  |
| ---- | ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| T    | 5     | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 0   | 0   |
| o    | 10    | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   |
| k    | 8     | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   | 0   |
| e    | 6     | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 0   |
| n    | 9     | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   |
| s    | 11    | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   |
|      | 0     | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
| i    | 7     | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   | 0   | 0   |
| n    | 9     | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   | 0   | 0   |
|      | 0     | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
| N    | 3     | 0   | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
| L    | 2     | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
| P    | 4     | 0   | 0   | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
| .    | 1     | 0   | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |