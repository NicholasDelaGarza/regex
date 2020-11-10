# Title (How to wright an e-mail code)

Introductory paragraph (replace this with your text)

I am Nicholas De La garza, this is my first tutorial and I chose to do it on matching an e-mail. if there is anything I am missing please comment 
## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

 The code example is: Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{3})$/.  Some example e-mails are (john.b.doe@gmail.com) and (jaindoe5@hotmail.org).

## Table of Contents

- [Anchors](#anchors)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components
Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{3})$/

### Anchors
/`^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{3})`$`/

The Anchors are the ^,$ symbols. The ^ goes in the front and the $ goes at the end. This is saying look at everything in between these two symbols.

### Character Classes
/^([a-z0-9_\.-]+)@([`\d`a-z`\.`-`]+)\.([a-z\.]{3})$/

 breaking down the character classes. We will start with \d: this matches single characters that is a digit, it is then followed by a-z. The a-z a long with \d can look for individual letters as well as words, what this means is if you put in say gmail or hotmail, it can pull out the (g) and then include the word (mail). For hotmail it can just combined the two words to make it valid.

Next is the \. this matches any character, so if the place you work has an internal e-mail system set up this can work to recognize any word, letter or symbol you put in there. This works with the – symbol, just a safety check to make sure that everything is caught.

There is a lot more to Character Classes so for more information please visit: https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285.
 
### Flags
`/`^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{3})$`/`

 The flags are the (/), this tells the code to look just within the to flags. Yes you need to make sure that you put one at the start right before the (^) and then at the end of ($). They work close to the same way as the Anchors, as they set the boundaries of your code. If you failed to put in the flags however and you have similar code before and after your e-mail address the system might get confused. So in short the flags set the boundaries of this code.

### Grouping and Capturing
/^`([a-z0-9_\.-]+)`@`([\da-z\.-]+)`\.`([a-z\.]{3})`$/

 Whatever you put inside of the () is how the code is going to be read and the order in which it will read it. I will explain Brackets next but for example with inside the () then you have brackets [] so it will execute that code first. Next it will move onto the +. The + symbol the way I see it is kind of like an (if) (else) statement. So you might have an e-mail that has (john.b.doe). So until it sees the @ symbol it will keep reading the code to make sure that it is valid. The @ symbol just tells the code to move on to the next set of grouping and capturing. I have already explained the next set in Character Classes and like that section if you want more info on this section just resort to that link previously provided. After the second section the \. is what tells the code to move on to the third section which I will cover in Greedy and Lazy Match.

### Bracket Expressions
/^(`[a-z0-9_\.-]`+)@(`[\da-z\.-]`+)\.(`[a-z\.]`{3})$/

Continuing from the previas section, Bracket Expressions is the part of the code that controls what it is looking for. In the first set of brackets it is looking for any letter or word from a-z, next it will search for any numbers from 0-9 even double digits, last it looks for everything else because of the \. Symbol as previously described. I have already described what is happening in the next set of brackets in the Character Classes section, so on to the third section. In this section it is just looking for any letter or number within a-z and then everything else with the use of \. Symbol.

### Greedy and Lazy Match
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]`{3}`)$/

 Most of this was coved in Bracket Expressions but let’s cover what the curly brackets mean. In this instance it is looking for just three letters, the ones that go at the end of an e-mail address. You know the .com, .gov, .edu and so on, some companies might even have there own but you still have to identify what you are looking for and this is how you do that. 

## Author

I'm nicholas de la garza and im a coder at the university of arizona. I hope you enjoyed my tutorial on matching my email.