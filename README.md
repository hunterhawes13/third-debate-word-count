## Synopsis

Third Presidential Debate word count using JavaScript to count the occurances of each word for both candidates and remove stop words. Stop words are natural language words which have very little meaning, such as "and", "the", "a", "an", and similar words.

###Trump most used words

country - 26 occurances
bad - 17 occurances
hillary - 17 occurances
great - 16 occurances
percent - 15 occurances
mosul - 15 occurances
years - 14 occurances
dollars - 14 occurances
money - 13 occurances
borders - 13 occurances
happened - 13 occurances
iran - 12 occurances
putin - 12 occurances
millions - 12 occurances
isis - 11 occurances
obama - 11 occurances
jobs - 11 occurances
states - 11 occurances
disaster - 10 occurances
trade - 10 occurances
border - 10 occurances
left - 10 occurances
start - 9 occurances
russia - 9 occurances
amendment - 9 occurances
lot - 9 occurances
countries - 9 occurances
president - 9 occurances
talk - 9 occurances
women - 8 occurances
wall - 8 occurances
tremendous - 8 occurances
justices - 8 occurances
wanted - 8 occurances
iraq - 8 occurances
big - 8 occurances
deals - 8 occurances
strong - 7 occurances
world - 7 occurances
started - 7 occurances
violence - 7 occurances
good - 7 occurances
united - 7 occurances
happen - 7 occurances
give - 6 occurances
billion - 6 occurances

###Clinton most used words

donald - 28 occurances
country - 25 occurances
president - 23 occurances
women - 22 occurances
jobs - 18 occurances
work - 15 occurances
american - 13 occurances
kind - 12 occurances
clear - 11 occurances
tax - 11 occurances
america - 11 occurances
debt - 11 occurances
security - 10 occurances
government - 10 occurances
chris - 10 occurances
syria - 10 occurances
court - 10 occurances
election - 10 occurances
world - 10 occurances
plan - 9 occurances
years - 9 occurances
economy - 9 occurances
families - 9 occurances
dollars - 9 occurances
immigrants - 9 occurances
trump - 9 occurances
undocumented - 9 occurances
million - 9 occurances
stand - 9 occurances
rights - 8 occurances
great - 8 occurances
that - 8 occurances
money - 7 occurances
amendment - 7 occurances
united - 7 occurances

## Code Example

```

//Find 'em!
var wordRegExp = /\w+(?:'\w{1,2})?/g;
var words = {};
var matches;
while ((matches = wordRegExp.exec(text)) != null)
{
    var word = matches[0].toLowerCase();
    if (typeof words[word] == "undefined")
    {
        words[word] = 1;
    }
    else
    {
        words[word]++;
    }
}

// Sort 'em!
var wordList = [];
for (var word in words)
{
    if (words.hasOwnProperty(word))
    {
        wordList.push([word, words[word]]);
    }
}
wordList.sort(function(a, b) { return b[1] - a[1]; });

// lets see what donny had to say
var n = 1187;
var message = ["The top " + n + " words are:"];
for (var i = 0; i < n; i++)
{
    message.push(wordList[i][0] + " - " + wordList[i][1] + " occurance" +
                 (wordList[i][1] == 1 ? "" : "s"));
}
console.log(message.join("\n"));
```

## Motivation

To compare the vocabulary and frequency of word use of the two candidates. Findings conclude that Trump used 779 words not considered stop words. Clinton 1186 words not considered stop words.
## Installation

<!---Provide code examples and explanations of how to get the project.-->

## API Reference

<!---Depending on the size of the project, if it is small and simple enough the reference docs can be added to the README. For medium size to larger projects it is important to at least provide a link to where the API reference docs live.-->

## Tests

<!---Describe and show how to run the tests with code examples.-->

## Contributors

Hunter Hawes
github: hunterhawes13
twitter: @tikishackfun

## License

This project is licensed under the terms of the MIT license.

## Warning

This should not be used in production. It is for demonstration purposes only.
