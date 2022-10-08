# RegEx

## . (character)

- find everything that is a character: string characters (normal or special), spaces, numbers.

## \d (digit) is equivalent to [0-9]

- find everything digit: numbers.

## \w (word) is equivalent to [a-zA-Z0-9_]

- find everything numbers and normal string character uppercase and lowercase, but without accent or spaces.

## \s (space)

- find spaces in the text. tabs included

## *, +, ? (delimiters)

- \* allows find zero or many
- \+ allows find one or many
- \? allows find zero or one

## {} (counters)

- is used to determine the minimum and maximum numbers of characters to find in a string.

### examples

+ \w{3} : sets that the minimum and maximum number of letters, numbers or underscores to find will be three (3).
+ \w{4, 6} : sets that the minimum will be four (4) and maximum will be six (6).
+ \w{5, } : sets that the minimum will be five (5) and maximum will be any higher amount.

## [] (classes)

- a class allows to define a personalizable pattern for searching and validations, to use classes, they must go inside the symbols [ ].

### examples

+ [A-Za-Z] : find any word regardless of whether it is uppercase or lowercase.
+ [A-Z0-7] : find any uppercase word or any number of between zero and seven.
## ^ (not)

- is used to negate an expression or invert it, is important that ^ (not) symbol is inside a class, if outside a class, the behavior is different, validating only the first character.

### examples

+ [^\w] is equivalen to [\W]: find everything that is not a word, number or underscore.
+ [^\d] is equivalen to [\D]: find everything that is not a digit.
+ [^\s] is equivalen to [\S]: find everything that is not a space.
+ ^[\w] is INVALID.

## start with ^ & end with $

- is used for validate the totally of a string, that is, the regex must match the entire string, not a part.

## \ (character escape)

- allows a special character to be found; example: [a-zA-Z\\.] allows find specifically . character and not any.