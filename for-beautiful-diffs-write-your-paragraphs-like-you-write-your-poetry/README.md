# For beautiful diffs, write your paragraphs like you write your poetry

This technique is currently kind of experimental. 
I personally haven't decided whether this should be a best practice or not.  
Help us debate this issue in the [issue queue](https://github.com/open-learning-exchange/GitHub-For-Writers-Manual/issues/1).
This post is written using this style guide except in places where it's intentionally not written like that for the sake of demonstration.

This is a technique used by Wired to write their "Lord of the Files" article.
You've grown up writing your paragraphs in word editors one line. 
This is promotes run on sentences and also makes your diffs very ugly to read.
Take these two seemingly identical paragraphs.


> The earliest known appearance of the phrase is from The Michigan School Moderator, a journal that provided teachers with education-related news and suggestions for lessons.[1] In an article titled "Interesting Notes" in the March 14, 1885 issue, the phrase is given as a suggestion for writing practice: "The following sentence makes a good copy for practice, as it contains every letter of the alphabet: 'A quick brown fox jumps over the lazy dog.'"[2] Note that the phrase in this case begins with the word "A" rather than "The". Several other early sources also use this variation.


> The earliest known appearance of the phrase is from The Michigan School Moderator, a journal that provided teachers with education-related news and suggestions for lessons.[1]
In an article titled "Interesting Notes" in the March 14, 1885 issue, the phrase is given as a suggestion for writing practice: "The following sentence makes a good copy for practice, as it contains every letter of the alphabet: 'A quick brown fox jumps over the lazy dog.'"
[2] Note that the phrase in this case begins with the word "A" rather than "The". 
Several other early sources also use this variation.


The difference you'll see if you check the raw source file is that first paragraph is a run on paragraph with only spaces between the sentences while the second paragraph has a line break between sentences yet it still shows up as a solid paragraph when rendered.  Note, make sure not to put spaces after your periods, that will actually cause the line to break!


This is useful especially when comparing revisions, otherwise known as looking at the diff (difference) between the saves.  
Here's are some examples of fixing the same typo in each of these paragraphs.  
See how much better the paragraph with line breaks looks?


I can spot the change in the second paragraph on the first paragraph without having to scroll left or right.
![I can spot the change in the second paragraph on the first paragraph without having to scroll left or right.](line-per-sentence--diff.png "I can spot the change in the second paragraph on the first paragraph without having to scroll left or right.")

The first paragraph scrolls to the right so far!
![The first paragraph scrolls to the right so far!](line-per-sentence--diff-runon.png)

Diff comments are line specific so with a paragraph that has each sentence on a line, we can target specific sentences with out comments.
![Diff comments are line specific so with a paragraph that has each sentence on a line, we can target specific sentences with out comments.](line-per-sentence--diff-comments.png)


