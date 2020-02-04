# Python - quick notes

## date-time
* `date.strftime(<date format>)` -> date to string
* `datetime.strptime(date_str, <date format>)` -> str to date

See also: 
* https://pythex.org/

## NNs

| Problem                                 | Activation  | Loss                     |
|-----------------------------------------|-------------|--------------------------|
| Binary classification                   | sigmoid     | Binary crossentropy      |
| Multiclass, single-label classification | softmax     | Categoric crossentropy   |
| Multiclass, multilabel classification   | sigmoid     | Binary crossentropy      |
| Regression                              | none        | MSE                      |
| Regration to 0-1 (1 node)|              | signoid     | MSE/binary cross entropy |


## regex
* `$`: match end.
* `^`: match start.


