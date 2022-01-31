# a-bad-wordle-solver
a somewhat questionable wordle solver using spreadsheets


Word Frequency uses the data given by _Rachael Tatman_ https://www.kaggle.com/rtatman/english-word-frequency. The 1/3 million words were filtered by length of 5 letters, then assigned a relative frequency score. This data was compared against the Wordle dataset and each solution word assigned the score given by the word frequency dataset.

Excel's 'Advanced Filter' function under the 'Data' tab is used to filter the words given by their result on Wordle:
* Green = letter and position match
* Orange = letter match, not position
* Grey = no letter match

Can then be filtered by Excel using:
* ?a??? - contains an 'a' in position 2
* \*a\* & <>??a?? - contains an 'a' not in position 3
* <>\*a\* - does not contain an 'a'
