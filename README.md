# wells-fargo-analytics

After cleaning the data using tm_map functions, I opted to turn the corpus back into a data frame to use in sentiment analysis.
There is a simple line of code in the webpage ...
new.df <- data.frame(text=unlist(sapply(docs, `[[`, "content")), stringsAsFactors=FALSE)
new.df$text is the column with all the posts and that is used for sentiment analysis.

I also turned each bank's corpus back into DF's.
new.df.BankA
new.df.BankB
new.df.BankC...

Instead of using the original df with no meta data taken out, new.df contains words that have real semantic meaning. This lends very well to sentiment analysis. And the new analysis builds on the differences between using the original data frame for sentiment analysis vs. the new (cleaned) data frame for sentiment analysis.
