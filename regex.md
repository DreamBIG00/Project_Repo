## Regex Concept
> Regex is the short of regular expression that aid searching and replacing operation on database. Regex is of great importance because it helps developer to identify patterns in a pool of data.
>
> Regular expressions (or regex, for short) are tools, and like all tools, regular expressions are designed to solve a very specific problem. The best
way to understand regular expressions and what they do is to understand
the problem they solve.
### Use case scenarios
_____
> * You are editing a source code and need to replace all occurrences of size with iSize, but only size and not size as part of
another word.
> * You are displaying a list of all files in your computer file system
and want to filter so that you locate only files containing the text
Application.
> * You are importing data into an application. The data is tab
delimited and your application supports CSV format files (one
row per line, comma-delimited values, each possibly enclosed
with quotes).
> * You need to search a file for some specific text, but only at a
specific location (perhaps at the start of a line or at the end of a
sentence).

>> All these scenarios present unique programming challenges. And all of
them can be solved in just about any language that supports conditional
processing and string manipulation. But how complex a task would the
solution become? You would need to loop through words or characters
one at a time, perform all sorts of if statement tests, track lots of flags so
as to know what you had found and what you had not, check for whitespace and special characters, and more. And you would need to do it all
manually.
>
>> Alternatively. one can avoid such stress and cumbersomneness with the help of regex. Each of the preceding challenges can be solved using well-crafted statements—highly concise strings containing text and special instructions—statements that may look like this: \b[Cc][Aa][Rr]\

>> **NB:** Regex is case sensitive

### Implementation of Regex
> Regex can be implemented in any scripting language like Ruby and co. Here we use Ruby to cite an example of implementing regex. Assuming we are to search an enrty from the standard input ( entering from the keyboard) for the word **school** in a text file say the first line read: *Agbo goes to school everyday*. We inmplement as follow:
> #### Ruby Script with .rb extension
>> ```ruby
 >> !#/usr/bin/env ruby
 >> puts ARGV[0].scan(/school/).join
>> ```
> #### Run Code
> > ```
>>./0-simply_match_school.rb Agbo goes to school everyday | cat -e
> > ```

> #### Output
> >```
>> school$
> >```

### Reference
> [Learn Regular expression in 10 minutes](https://zlibrary-ng.se/book/10991885/ddc391)

### Author
> **Ovwiurhobo Holy** ([email](oghenewonaholy@gmail.com))
