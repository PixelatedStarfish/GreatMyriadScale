
# The Great Myriad Scale

Say for the sake of argument, you want to invent a new way to count. Maybe you had had a lot of counting to do, reps, days, sheep. Maybe you just need some way to spice things up. So, you start counting with the largest numbers you can name. Then, you run out of names, so you make up names, like a little kid would. Unlike a little kid, you actually start doing the counting homework, the math and research. You read about Archimedes, with his myriads of sand. You read about the Conway-Weschler system of "millinillions" which extend the Adam-Chuquet "millions". Oh! Kyoda, wrote a computer program, called "Conway’s illion Converter". How nice! While you are abusing that program, you watch the names get long, very, very long. Strings of Latin stretch out, past the edges of your screen, then, out of your screen, and into your room, onto your walls, and out your windows. Then, they double back! The numbers are getting supernatural, tying up in Knuth-ish knots of chaining arrows, bounding, bouncing, bowering about. It is all becoming too much! 

New plan, drop the millions. You can still count from one to ten, to twenty-five, to one hundred. You can count to one thousand, and to one-hundred-thousand, with products on the left of "thousand" and sums on the right. You can even count to one-thousand-thousand, but that needs a new name.  You try a "second thousand" and a third, and a fourth. How do you say that? Well, "fourth degree thousand" works. Hold that thought. Myriads work. They play nicely with "fourth" and "fifth", and all other oridnals. Okay, one-hundred-hundred is a myriad, and a squared myriad is a "second (degree) myriad". Multiply that by one hundred for "one hundred of the second myriad" and again for "one third myriad". The "one hundred second myriad" is a much larger number, not to be confused. Also, you need a word for "hundredth hundred" or "myriadth myriad. Okay, introduce "great" for "great hundred" and "great myriad". Great, but this is still all quite wordy. You think would be nice to consolidate some of these long strings into fewer words, before you start on with "great, great myriad", or "myriad of two greats". (How recursive!) Should you use some more Greek? "Deuteros" means "second". "Deuteros Myriad" can be shortened to deut-yriad. New word, "deutyriad", like a Greek-ish "billion" Oh boy, nomenclature. Keep going and you have a new (reinvented) scale. You have a "Great Myriad Scale". (Now python implemented, check the sources.)[1][2][3][4]


## Design of the Great Myriad Scale

So you might be wondering what makes this project a scale, rather than a list of arbitrary numbers and made up names? The Great Myriad Scale was written with design criteria in mind, to achieve a primary goal: this scale should actually be countable. Someone should be able to start from one and (given enough time) count all of the natural numbers, one by one, two, three, all the way to the largest denominations, and on to infinity; every number in between one and a Great Myriad should have a useful name, constructed from a set of denominations:

* Denominations are numbers whose names can be used to construct the names of other numbers, including one, ten, one hundred, one thousand, one myriad, and larger derivatives...

* The value of a denomination is constant. "One Hundred" always refers to 100, the square of ten. Name conflicts are not allowed. Names must be distinct, and pronounceable. So arbitrary names like "abcd" or "wxyz" are not allowed.   

* The names of non-denominational numbers are constructed from denominations: largest in the middle, products on the left, and sums on the right; (2 * 100 + 3) is "two hundred three".

* Denominations are always named according to one consistent scheme, which is constant throughout the entire scale. This scheme is not arbitrary, but based on a denomination, and compared to it with minimal edge cases. This includes naming powers of the myriad with Latinized Ancient Greek, or powers of the million with Latin. In these examples, larger denominations share an etymology with the denomination on which they are based.

* A denomination can be no larger than the square of a preceding, smaller denomination (with exception for denominations which are there own squares). In other words "one myriad, myriad, myriad" is just verbose, so is best to name that something shorter. Of course, there are only so many arrangements of letters, so a largest denomination must eventually be reached, but all smaller denominations that can follow this rule, will follow this rule.


## Defining the Myriad

First off, what is a myriad? So, one hundred is the square of ten, and one myriad is the square of one hundred. In other words, a myriad is equal to ten to the power of four (1,0000). Commas group four digits in this scale, so the square of a myriad is written as (1,0000,0000) What is the square of a myriad called? We will get to that. Let's start with a table to count from one to one myriad:

| n  | Name   | n  | Name       | n      | Name                       |      
|----|--------|----|------------|--------|----------------------------|
| 1  | One    | 12 | Twelve     | 30     | Thirty                     |
| 2  | Two    | 13 | Thirteen   | 40     | Forty                      |
| 3  | Three  | 14 | Fourteen   | 50     | Fifty                      |
| 4  | Four   | 15 | Fifteen    | 60     | Sixty                      |
| 5  | Five   | 16 | Sixteen    | 70     | Seventy                    |
| 6  | Six    | 17 | Seventeen  | 80     | Eighty                     |
| 7  | Seven  | 18 | Eighteen   | 90     | Ninety                     |
| 8  | Eight  | 19 | Nineteen   | 100    | One Hundred                |
| 9  | Nine   | 20 | Twenty     | 500    | Five Hundred               |
| 10 | Ten    | 21 | Twenty One | 1000   | Ten Hundred (One Thousand) |
| 11 | Eleven | 22 | Twenty Two | 1,0000 | One Myriad  (Ten Thousand) |

You may notice the "ten hundred" there, and think it sounds a bit odd. Both "ten hundreds" and "one thousands" are acceptable in this scale. As a guideline, thousands as best used for rounded thousands under ten to the fifth power (ten myriad). Rounded thousands are integers with zeroes in units, tens, and hundreds place ("five thousand"). If a thousand is not round, use hundreds ("fifteen hundred"). At ten to the fifth, switch to myriads. That said, this project is not intended to argue that the way you count is wrong. In other words, the Great Myriad Scale is not intended to be sold as "counting 2.0 - new and improved in every way". Instead this scale is intended as another tool in your kit, something to make those large numbers easier to deal with. Now it's time to get to that square of a myriad, and the larger powers. [5]


## The Myriad Powers

In this scale each power of the myriad get a Greek prefix and an "-yriad" suffix. For example "deutyriad" is a myriad to the second power. it is named by shortening "deuteros myriad", with "deuteros" referring to "second". Each successive power follows this scheme:   

|   e | Name              |   e | Name                  |     e | Name                    |
|----:|:------------------|----:|:----------------------|------:|:------------------------|
|   4 | One Myriad        |  48 | One Dodecatyriad      |   120 | One Tricostyriad        |
|   8 | One Deutyriad     |  52 | One Decatotrityriad   |   160 | One Tesserecostyriad    |
|  12 | One Trityriad     |  56 | One Decatotetyriad    |   200 | One Pentecostyriad      |
|  16 | One Tetyriad      |  60 | One Decatopemptyriad  |   240 | One Hexecostyriad       |
|  20 | One Pemptyriad    |  64 | One Decatohectyriad   |   280 | One Hebdomecostyriad    |
|  24 | One Hectyriad     |  68 | One Decatohebdomyriad |   320 | One Ogdoecostyriad      |
|  28 | One Hebdomyriad   |  72 | One Decatogdyriad     |   360 | One Enatecostyriad      |
|  32 | One Ogdyriad      |  76 | One Decatenatyriad    |   400 | One Hecatostyriad       |
|  36 | One Enatyriad     |  80 | One Icostyriad        |  2000 | One Pentehecatostyriad  |
|  40 | One Decatyriad    |  84 | One Icostoprotyriad   |  4000 | One Decatehecatostyriad |
|  44 | One Hendecatyriad |  88 | One Icostodeutyriad   | 40000 | One Great Myriad        |

Each power of the myriad is named in this pattern until the Great Myriad, which gives this scale its name. The Great Myriad is equal to the myriad raised to the power of a myriad, which is ten to the power of four myriad. Is that it? No, of course there is more to discuss. The "Myriad Great Myriad" is equal to a Great Myriad times a myriad. A Great Myriad times a deutyriad is a "Deutyriad Great Myriad". Square a Great Myriad for a Great Deutyriad. Cube it for a Great Trityriad, and so on. Of course, by raising the Great Myriad to the power of a myriad, we get a "Great, Great Myriad". Raise this to the power of a myriad again to get  a "Great, Great, Great Myriad" and so on. To keep names short, an adverbial naming scheme is used. The "Great, Great Myriad" is called the "Two-fold Greater Myriad". The "Great, Great, Great Myriad" is called the "Three-fold Greater Myriad", and so on. Eventually the "Myriad-fold Greater Myriad" is reached, which is followed by the "Deutyriad-fold Greater Myriad". Even the "Greater-Myriad-fold Greater Myriad" can be reached, in addition to the "Two-fold-Greater-Myriad-fold Greater Myriad". You are free to count right up to infinity this way. [5][6]


## Constructing Cardinals, Ordinals, and Fractions

Counting the cardinal numbers between large myriads is done as it would be for any conventional denomination: largest in the middle, multipliers on the left, sums on the right. For example, one hundred times two, plus two is "two hundred, two" or "two hundred and two". Therefore, A great myriad times a myriad is a "myriad great myriad". Add one hundred to this and you get "one myriad, great myriad, one hundred".

Ordinals are used for listing items; such as first, second, and third. The ordinals below the myriad are conventional: cardinal "ten" is paired with ordinal "tenth", hundred is paired with hundredth, thousand is paired with thousandth. Thus, cardinal "myriad" is paired with "myriadth", "deutyriad" with "deutyriadth", and "great myriad" with "great myriadth". Each cardinal has an ordinal, and these ordinals can be used to denote fractions (in the same manner that ordinals are conventionally used). One over a great myriad is "one great myriadth". Double that for "two great myraidths", and so on.  

If you want to describe something like (1/3) * 1,0000,0000,0000; you can refer to it as a "third of a trityriad" or "one third of a third degree myriad". Admittedly, if you are using oridnals to describe powers of a myriad, you may need to explicitly specify ordinals that refer to fractional parts, as in "fractional fourth of a myriad" compared to "fourth degree myriad".[6]


## Counting in Languages

Do not assume that because this document is written in American English, the Great Myriad Scale is only usable in American English. All terms coined are intended to be translated in about the same manner one would translate an English cardinal or ordinal number. If you use *myriad*, *myriade*, or *miriada*; then you would use *deutyriad*, *deutyriade*, or *deutiada* (assuming Google translate has accurately translated "myriad" into French and Spanish). Similarly, *Great* may translate to *Grande*, or *Grande*; *Tenfold* to *Diez veces* or *Dix fois*. Modify the nomenclature as required. 


## Scale Variations

Say, for the sake of argument, that you really like the short scale, but not the Latin. You want to count with powers of one thousand, rather than powers of one myriad, or of one million. Well, you can use "chilliads" to count in the "Great Chilliad" Scale. "Chilliad" refers to one thousand, and the square of one thousand would be a "deuterilliad", from "deuteros-chilliad". You can then substitute the third power for "tritilliad", from "Tritos-Chilliad" and continue on accordingly.

If you instead want a super long scale, you can be like mathematician Donald Knuth, and set each new denomination to the square of the previous one. One hundred is the square of ten, and one myriad is the square of one hundred. Then, in Knuth's "Supernatural Numbers", "one myllion" is the square of one myriad, and the square of that is a "byllion". It's easy to rename the "myllion" to a "deutyriad", and the "byllion" to a "trityriad", and then continue onward to construct a "Supernatural Myriad Scale". [7]


## Why?

Well, there are only so many names, there can only be so much wordplay. To keep all the numbers countable, their names needed to be constructed from smaller numbers. Sure, you can start naming with hyperoperations, but they grow faster, and faster and soon you have an unstable scaffold stretched over growing, turbulent voids ever more difficult to bridge. If you cannot count to a number, then such a number is really a vague suggestion of magnitude, a dream of many zeroes... Oh, you meant "Why invent this counting scale thing anyway? Millions are fine, and we already have scientific notation, and who would ever count from one to 'greater-myriad-fold greater myriad' anyway?" Well, have you ever played one of those incremental video games, with all the numbers going up to astronomical absurdity? You wake up to "Hey, while you were sleeping, you got twenty quattuorvigintillion points in the tower of tumbleweeds!", and you remember all the sheep you counted last night, hoping for rest, because in the morning, you have a fracture to tend. You have to prevent muscular atrophy by isometrically flexing a muscle several hundred times, and that means even more counting. 

So you make up new names for new numbers, to spice it up. You ask yourself "Where do all the number names come from anyway, and when do we run out?" and you begin researching and lo, the rabbit hole! It opens before you to a wonderland of Latin and "googology", and before you realize it you have let the number goblins in. They shout "We want an incremental game! One where players can read all the numbers!" They jump on the bed. "Notations! Bah! Fie on notations!" The number goblins demand a sense of scale. "Notations transform orders of magnitude into mere increments! Madness! People need names! Names!" They grab hold of the bed knobs and shake. The leader shouts in your ear "Don't you understand?! Do it for Archimedes!" The chanting begins. "Conway! Weschler! Knuth!". You are surrounded in a cacophonous, cantankerous, chorus of contention! Then, in unison, a deep breath, and the call of a great horn. Then you hear it, "Millinillinillinillinyllion!" With this incantation you are changed, goblinified! There is only one way to lift the spell! Give them their tables, and their powers of ten, so that they might count in numerological novelty until the end of all things! Of course, you accept the mission, and by the time you are healed, you have finished some sort of hobbyist research paper on numeric conjecture, complete with a nice little implementation for the goblins to play with. 


## Proof of the Great Myriad Scale

All of this discussion of counting has attracted the attention of a Number Goblin. They seem unimpressed by the tables, wordplay, and implementation. They sneer at the coinages, the portmanteaus, and the liberties taken with Ancient Greek. "Enatecostos? I think you mean 'enenekostos'. Pentehecatostos? Fie! You mean 'pentakosiostos'. I do not trust your wordplay, your tables, not your rules, not your implementation. Not yet! A bit of recursion and concatination is not going to convince me that easily!" The Goblin issues a challenge: "You will prove you can count in arbitrary succesion. You will do so without reliance on scales, or languages. You will count with the absolute minimum of vocabulary, in base ten, with a unique name for each succeding natural number!"

You must begin, with no other choice, you start with calling 1, "one". One is succeded by "two", then "three", then "four", then "five", "six", "seven", "eight", "nine", and then "ten", with each named as directed by the Goblin. With that, you have named every natural number out to 10, in base ten. You pause. "What comes next?" the Goblin demands. "Eleven", you say, a mistake. "No!", the Goblin screams "Minimize required vocabulary!" Obliged, you decide that "ten" must be succeeded by "ten-one". This pleases the Goblin. They watch you count to "ten-nine" with a smile, naming each natural number in succession. Having reached 20, you pause again, and begin to say "twen-", "No!" the Goblin interupts with a screech. "Two-ten! Got it?! Two-ten! Now, what comes after that?!". You reply with "Two-ten-one", speaking in a careful, trembling, whisper. "Good! Now proceed!" the Goblin urges with a toothy grin. Again, you continue, to "two-ten-nine" for 29, past "three-ten" (30), and "four-ten-two" (42), and just after "nine-ten-nine" (99), you hear "Stop!" cutting in. "You were about to say 'ten-ten' a name much too ambiguous to use! It could refer to 20 or to 100, if no context is provided! This cannot do!" The Goblin thinks, with a scratch of long nails on a scaly chin. You inhale to speak, but not as quickly as the Goblin. "I will now provide you with levity! Accept this generous offer of a new word to the vocabulary. I call it 'hundred', and you will call 100 'hundred'. You will be provided with a new word at the square of this denomination. Now, rejoice!" 

You continue on, counting "hundred-one" (101), and "hundred-two" (102). You count past "hundred-two-ten" (120), and reach "two-hundred" (200), in a manner similar to your method for counting to "hundred". Then you count through the hundreds, successively, over a few hours. You count past "two-ten-hundred" (2000), and "five-ten-five-hundred-five-ten-five" (5555). The Goblin is silent, but watching intently. You have not the chance to notice the blinking of their eyes, as you count to "nine-ten-nine-hundred-nine-ten-nine" (9999). "Myriad! 10000 will be called the 'myriad'". As with "ten", and "hundred", you begin to proceed to the next square, but you realize that is going to take several weeks. You stop. The Goblin begins to speak, but you best them to it. "'Myriamyriad!' That would be the name for 100000000! The square of that is twice as verbose, 'myriamyriamyriamyriad!' The next square is the 'myriamyriamyriamyriamyriamyriamyriamyriad!' Is that not proof enough?! Can we please use a scale now?!". Time passes, and the Goblin relents. "Very well, you are quite repetitive without one. This will be of great help to our quest. You are free." and so the Goblin vanishes into digits, with a parting remark: "For fractions, you can use 'over' as in 'one-over-five!'" 


## Footnotes and (Additional) Trivia

* Strictly employing Ancient Greek ordinals is, in a word, challenging. There are conflicting uses of ordinal and cardinal forms, which is to say nothing of the challenges of conflicting transliterations. Nomenclature was chosen to minimize exceptional namings or spellings.
* You can certainly call infinity the "Apyriad" if you wish. The "Apyriad" is derived from "apeiro".[5]
* Archimedes' largest Sand Number (the largest described in The Sand Reckoner) is equal to 10^(8 * 10^16), or a "Four-fold Greater Deutyriad".[8]
* "Cola's Enumeration" and the "Ordinal Myriad Scale" are previous attempts to enumerate large numbers, using the Conway Wechsler system, Greek ordinals, and hyperoperations. Ultimately, it is important that each name for a large number is based on the names of smaller numbers, rather than operations or notations. The numbers between "novel numbers", or "milestone numbers", also need to be nameable.


## Tables

Nomenclature Table[5][6]

| n  | Name         | n  | Name            | n      | Name                          |    
|----|--------------|----|-----------------|--------|-------------------------------|
| 1  | Protos       | 12 | Dodecatos       | 30     | Tricostos                     |
| 2  | Deuteros     | 13 | Decatotritos    | 40     | Tesserecostos                 |
| 3  | Tritos       | 14 | Decatotesseros  | 50     | Pentecostos                   |
| 4  | Tetaros      | 15 | Decatopemptos   | 60     | Hexecostos                    |
| 5  | Pemptos      | 16 | Decatohectos    | 70     | Hebdomecostos                 |
| 6  | Hectos       | 17 | Decatohebdomos  | 80     | Ogdoecostos                   |
| 7  | Hebdomos     | 18 | Decatogdoos     | 90     | Enatecostos                   |
| 8  | Ogdoos       | 19 | Decatenatos     | 100    | Hecatostos                    |
| 9  | Enatos       | 20 | Icostos         | 500    | Pentehecatostos               |
| 10 | Decatos      | 21 | Icostoprotos    | 1000   | Decatehecatostos (Chiliostos) |
| 11 | Hendecatos   | 22 | Icostodeuteros  | 10000  | Myriad (Myriastos)            |


Sub-myriad Table[5] 

| n  | Name   | n  | Name       | n      | Name                       |      
|----|--------|----|------------|--------|----------------------------|
| 1  | One    | 12 | Twelve     | 30     | Thirty                     |
| 2  | Two    | 13 | Thirteen   | 40     | Forty                      |
| 3  | Three  | 14 | Fourteen   | 50     | Fifty                      |
| 4  | Four   | 15 | Fifteen    | 60     | Sixty                      |
| 5  | Five   | 16 | Sixteen    | 70     | Seventy                    |
| 6  | Six    | 17 | Seventeen  | 80     | Eighty                     |
| 7  | Seven  | 18 | Eighteen   | 90     | Ninety                     |
| 8  | Eight  | 19 | Nineteen   | 100    | One Hundred                |
| 9  | Nine   | 20 | Twenty     | 500    | Five Hundred               |
| 10 | Ten    | 21 | Twenty One | 1000   | Ten Hundred (One Thousand) |
| 11 | Eleven | 22 | Twenty Two | 1,0000 | One Myriad                 |


The Myriad Powers[5][6]

|   e | Name              |   e | Name                  |     e | Name                    |
|----:|:------------------|----:|:----------------------|------:|:------------------------|
|   4 | One Myriad        |  48 | One Dodecatyriad      |   120 | One Tricostyriad        |
|   8 | One Deutyriad     |  52 | One Decatotrityriad   |   160 | One Tesserecostyriad    |
|  12 | One Trityriad     |  56 | One Decatotetyriad    |   200 | One Pentecostyriad      |
|  16 | One Tetyriad      |  60 | One Decatopemptyriad  |   240 | One Hexecostyriad       |
|  20 | One Pemptyriad    |  64 | One Decatohectyriad   |   280 | One Hebdomecostyriad    |
|  24 | One Hectyriad     |  68 | One Decatohebdomyriad |   320 | One Ogdoecostyriad      |
|  28 | One Hebdomyriad   |  72 | One Decatogdyriad     |   360 | One Enatecostyriad      |
|  32 | One Ogdyriad      |  76 | One Decatenatyriad    |   400 | One Hecatostyriad       |
|  36 | One Enatyriad     |  80 | One Icostyriad        |  2000 | One Pentehecatostyriad  |
|  40 | One Decatyriad    |  84 | One Icostoprotyriad   |  4000 | One Decatehecatostyriad |
|  44 | One Hendecatyriad |  88 | One Icostodeutyriad   | 40000 | One Great Myriad        |


Table of Scales[2][3][4][5][6]

|     e | Great Myriad Scale             | Conway-Weschler Short                           | Conway-Weschler Long                             |
|------:|:-------------------------------|:------------------------------------------------|:-------------------------------------------------|
|     0 | One                            | One                                             | One                                              |
|     1 | Ten                            | Ten                                             | Ten                                              |
|     2 | One Hundred                    | One Hundred                                     | One Hundred                                      |
|     3 | Ten Hundred                    | One Thousand                                    | One Thousand                                     |
|     4 | One Myriad                     | Ten Thousand                                    | Ten Thousand                                     |
|     5 | Ten Myriad                     | One Hundred Thousand                            | One Hundred Thousand                             |
|     6 | One Hundred Myriad             | One Million                                     | One Million                                      |
|     7 | Ten Hundred Myriad             | Ten Million                                     | Ten Million                                      |
|     8 | One Deutyriad                  | One Hundred Million                             | One Hundred Million                              |
|    12 | One Trityriad                  | One Trillion                                    | One Billion                                      |
|    16 | One Tetyriad                   | Ten Quadrillion                                 | Ten Thousand Billion                             |
|    20 | One Pemptyriad                 | One Hundred Quintillion                         | One Hundred Trillion                             |
|    24 | One Hectyriad                  | One Septillion                                  | One Quadrillion                                  |
|    28 | One Hebdomyriad                | Ten Octillion                                   | Ten Thousand Quadrillion                         |
|    32 | One Ogdyriad                   | One Hundred Nonillion                           | One Hundred Quintillion                          |
|    36 | One Enatyriad                  | One Undecillion                                 | One Sextillion                                   |
|    40 | One Decatyriad                 | Ten Duodecillion                                | Ten Thousand Sextillion                          |
|    44 | One Hendecatyriad              | One Hundred Tredecillion                        | One Hundred Septillion                           |
|    48 | One Dodecatyriad               | One Quindecillion                               | One Octillion                                    |
|    52 | One Decatotrityriad            | Ten Sedecillion                                 | Ten Thousand Octillion                           |
|    56 | One Decatotetyriad             | One Hundred Septendecillion                     | One Hundred Nonillion                            |
|    60 | One Decatopemptyriad           | One Novendecillion                              | One Decillion                                    |
|    64 | One Decatohectyriad            | Ten Vigintillion                                | Ten Thousand Decillion                           |
|    68 | One Decatohebdomyriad          | One Hundred Unvigintillion                      | One Hundred Undecillion                          |
|    72 | One Decatogdyriad              | One Tresvigintillion                            | One Duodecillion                                 |
|    76 | One Decatenatyriad             | Ten Quattuorvigintillion                        | Ten Thousand Duodecillion                        |
|    80 | One Icostyriad                 | One Hundred Quinvigintillion                    | One Hundred Tredecillion                         |
|    84 | One Icostoprotyriad            | One Septemvigintillion                          | One Quattuordecillion                            |
|    88 | One Icostodeutyriad            | Ten Octovigintillion                            | Ten Thousand Quattuordecillion                   |
|    92 | One Icostotrityriad            | One Hundred Novemvigintillion                   | One Hundred Quindecillion                        |
|    96 | One Icostotetyriad             | One Untrigintillion                             | One Sedecillion                                  |
|   100 | One Icostopemptyriad           | Ten Duotrigintillion                            | Ten Thousand Sedecillion                         |
|   200 | One Pentecostyriad             | One Hundred Quinsexagintillion                  | One Hundred Trestrigintillion                    |
|   400 | One Hecatostyriad              | Ten Duotrigintacentillion                       | Ten Thousand Sesexagintillion                    |
|   404 | One Hecatostprotyriad          | One Hundred Trestrigintacentillion              | One Hundred Septensexagintillion                 |
|   800 | One Deuterehecatostyriad       | One Hundred Quinsexagintaducentillion           | One Hundred Trestrigintacentillion               |
|  1200 | One Tritehecatostyriad         | One Novenonagintatrecentillion                  | One Ducentillion                                 |
|  1600 | One Tesserehecatostyriad       | Ten Duotrigintaquingentillion                   | Ten Thousand Sesexagintaducentillion             |
|  2000 | One Pentehecatostyriad         | One Hundred Quinsexagintasescentillion          | One Hundred Trestrigintatrecentillion            |
|  2400 | One Hexehecatostyriad          | One Novenonagintaseptingentillion               | One Quadringentillion                            |
|  2800 | One Hebdomehecatostyriad       | Ten Duotrigintanongentillion                    | Ten Thousand Sesexagintaquadringentillion        |
|  3200 | One Ogdoehecatostyriad         | One Hundred Milliquinsexagintillion             | One Hundred Trestrigintaquingentillion           |
|  3600 | One Enatehecatostyriad         | One Millinovenonagintacentillion                | One Sescentillion                                |
|  4000 | One Decatehecatostyriad        | Ten Milliduotrigintatrecentillion               | Ten Thousand Sesexagintasescentillion            |
|  4400 | One Hendecatehecatostyriad     | One Hundred Milliquinsexagintaquadringentillion | One Hundred Trestrigintaseptingentillion         |
|  4800 | One Dodecatehecatostyriad      | One Millinovenonagintaquingentillion            | One Octingentillion                              |
|  5200 | One Decatetritehecatostyriad   | Ten Milliduotrigintaseptingentillion            | Ten Thousand Sesexagintaoctingentillion          |
|  5600 | One Decatetesserehecatostyriad | One Hundred Milliquinsexagintaoctingentillion   | One Hundred Trestrigintanongentillion            |
|  6000 | One Decatepentehecatostyriad   | One Millinovenonagintanongentillion             | One Millinillion                                 |
|  6400 | One Decatehexehecatostyriad    | Ten Billiduotrigintacentillion                  | Ten Thousand Millisesexagintillion               |
|  6800 | One Decatehebdomehecatostyriad | One Hundred Billiquinsexagintaducentillion      | One Hundred Millitrestrigintacentillion          |
|  7200 | One Decatogdoehecatostyriad    | One Billinovenonagintatrecentillion             | One Milliducentillion                            |
|  7600 | One Decatenatehecatostyriad    | Ten Billiduotrigintaquingentillion              | Ten Thousand Millisesexagintaducentillion        |
|  8000 | One Icostehecatostyriad        | One Hundred Billiquinsexagintasescentillion     | One Hundred Millitrestrigintatrecentillion       |
|  8400 | One Icosteprotehecatostyriad   | One Billinovenonagintaseptingentillion          | One Milliquadringentillion                       |
|  8800 | One Icostedeuterehecatostyriad | Ten Billiduotrigintanongentillion               | Ten Thousand Millisesexagintaquadringentillion   |
|  9200 | One Icostetritehecatostyriad   | One Hundred Trilliquinsexagintillion            | One Hundred Millitrestrigintaquingentillion      |
|  9600 | One Icostetesserehecatostyriad | One Trillinovenonagintacentillion               | One Millisescentillion                           |
| 10000 | One Icostepentehecatostyriad   | Ten Trilliduotrigintatrecentillion              | Ten Thousand Millisesexagintasescentillion       |
| 20000 | One Pentecostehecatostyriad    | One Hundred Sextilliquinsexagintasescentillion  | One Hundred Trillitrestrigintatrecentillion      |
| 40000 | One Great Myriad               | Ten Tredecilliduotrigintatrecentillion          | Ten Thousand Sextillisesexagintasescentillion    |
| 40004 | One Myriad Great Myriad        | One Hundred Tredecillitrestrigintatrecentillion | One Hundred Sextilliseptensexagintasescentillion |


## Sources

* [1] [Github Repository for this Page](https://github.com/PixelatedStarfish/GreatMyriadScale)
* [2] [Conway's illion Converter and the Conway-Weschler System](https://kyodaisuu.github.io/illion/conway.html)
* [3] [Long and Short Scales](https://en.wikipedia.org/wiki/Long_and_short_scales)
* [4] [Myriad](https://en.wikipedia.org/wiki/Myriad)
* [5] [List of Polygons](https://en.wikipedia.org/wiki/List_of_polygons)
* [6] [Ancient Greek Numbers](https://en.wiktionary.org/wiki/%CF%84%CE%AD%CF%83%CF%83%CE%B1%CF%81%CE%B5%CF%82)
* [7] [Knuth's Supernatural Numbers](https://mrob.com/pub/math/largenum-2.html#yllion)
* [8] [Archimedes' Sand Number](https://en.wikipedia.org/wiki/The_Sand_Reckoner)