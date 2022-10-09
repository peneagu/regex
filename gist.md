Regex Tutorial

Have you ever wondered what happens when you click the "filter" check boxes on a web page? Without having to spend hours on the same screen, It can be used to look for information through large bodies of information and even help validate if the information entered is correct. Regex is a combination of symbols that informs the computer what to find, what not to find, and any type of limits one might want to impose in their search.

Summary
Regex expressions are made of a myriad of components. This tutorial will cover regular expression, or Regex, basics of meta characters.

Table of Contents
Character Sets
Bracket Expressions
The Period
Repetitions
The Star
The Plus
The Question Mark

 
Character Sets
Character classes, also called character sets, are stored as binary numbers because computers work in binary.  Square brackets are used to specify character sets. To specify the characters' range, use a hyphen inside a character set. However, remember that the order of the character range inside the square brackets doesn't matter. For example, the regular expression [Tt]he means: an uppercase T or lowercase t, followed by the letter h, followed by the letter e.

"[Tt]he" => The girl went to the mall.

A period inside a character set, however, means a literal period. The regular expression ar[.] means: a lowercase character a, followed by the letter r, followed by a period . character.

"ar[.]" => A shady spot is good place to park a car.

Repetitions
To decide how many times a sub-pattern can occur, the meta characters +, * or ? are used. These meta characters act differently in different situations.

The Star
The regular expression a* means: zero or more repetitions of the preceding lowercase character a; or more repetitions of whatever preceding matcher. When the regular expression [a-z]* means: any number of lowercase letters in a row. So, if it appears after a character set or class then it finds the repetitions of the whole character set.

"[a-z]*" => The car parked in the space #58.

The Plus
The regular expression c.+t means: a lowercase c, followed by at least one character, followed by a lowercase t. So, the + symbol matches one or more repetitions of the preceding character.  It does need to be clarified that it is the last t in the sentence.

"c.+t" => The cat sat on the mat.

The Question Mark
In regular expressions, this symbol matches zero or one instance of the preceding character. The regular expression [T]?he means: Optional uppercase T, followed by a lowercase h, followed by a lowercase e. In other words, the meta character ? makes the preceding character optional.

"[T]he" => The car is parked in a shady spot.

"[T]?he" => The car is parked a shady spot.