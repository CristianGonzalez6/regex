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


## \ (character escape)

- allows a special character to be found; example: [a-zA-Z\\.] allows find specifically . character and not any.