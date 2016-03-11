# rule-based-classifier

pos.wn(positive wordnet items) and neg.wn(negative wordnet items) files contain positive and negative words extracted from SentiWordnet, http://sentiwordnet.isti.cnr.it/ (original source) and you can acquire it from the authors. These files are used under a license and cannot be shared.

The format of each of the file is one word or phrase per line. Phrases are concatenated with an underscore (so we cleaned up the data a little bit and can be done by a script or use unix to replace the underscore with a space).

For example, you have the phrase "twilight_of_the_gods" in the neg.wn file.

In “Data," you have 1000 posTweets.txt (with 1000 tweets with a ":)" face

 
and 1000 negTweets.txt (with 1000 tweets with a ":(" face)
 
You also have a third file from Twitter that has the following format:
 
— Emotion label (e.g., “HAPPY”, “ANGRY”) \t Tweet_id \t Tweet_text
 
Task: We built a rule-based classifier for sentiment (or emotion, although we still don’t have emotion dictionaries). Basically we count the positive words and/or negative words (based on the dictionaries pos.wn and neg.wn) in each sentence and will be able to decide whether a sentence is positive or negative, or mixed (if it has both positive and negative words). 
