# Text-Summarizer
How to use:

Simply call the Summarize(String text, int maxSummarySize) method. Pass in your text, and pass in how many sentences you want your summary to be.

**Here's how it works**

1. Start by recording raw frequencies of words within the text. Ideally, a Map works best for this. 
2. Next, any stopwords within the Map are filtered and removed; so as to reduce redundancy and keep only certain key phrases and words. 
3. After, sort the Map, from greatest word frequency to least. 
4. Then, get sentences from your original text, formatting and making sure any abbreviations and suffixes with a period or decimal are not counted as the ending of a sentence. 
5. Next, for text that is from online, we need to format and adjust it so that certain un-needed text is removed. 
6. Finally, obtain the summary by going through your list of sentences (from step 4) and then using your Map, compare and find the key phrases and words from each sentence. If found, add that sentence to the summary list.
7. Once all done, return the summary as a String. 
