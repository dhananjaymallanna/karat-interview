Write a function to output fully justified text. The output must be an array of lines, and each line must have length equal to "lineLength" parameter - except if it's just one word. See Examples:

# Example 1 input
text = [ "Some modern typesetting programs",
          "offer four justification",
          "options" ]
lineLength = 24

# Your function, justify(text, lineLength)
# should return:
       [ "Some  modern typesetting",
         "programs    offer   four",
         "justification    options" ]
Within the same line, the amount of spaces between words should differ by no more than 1 space:

Not Allowed: "the      quick brown fox"
    Allowed: "the   quick   brown  fox"
Example 2:

# input
text = [ "The Earth is",
         "the only world",
         "known so far",
         "to harbor life" ]
lineLength = 18

# Return:
       [ "The  Earth  is the",
         "only  world  known",
         "so  far  to harbor",
         "life" ]
Example 3:

# input
text = [ "It underscores our responsibility",
         "to deal more kindly with one another" ]
lineLength = 15

# Return:
       [ "It  underscores",
         "our",
         "responsibility",
         "to   deal  more",
         "kindly with one",
         "another" ]
This problem is similar to, but not exactly the same as the problem https://leetcode.com/problems/text-justification/
