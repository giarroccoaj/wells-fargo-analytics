# wells-fargo-analytics

After cleaning the data using tm_map functions, I opted to turn the corpus back into a data frame to use in sentiment analysis.
There is a simple line of code in the webpage ...
new.df <- data.frame(text=unlist(sapply(docs, `[[`, "content")), stringsAsFactors=FALSE)
new.df$text is the column with all the posts and that is used for sentiment analysis.

Instead of using the original df with no meta data taken out, new.df contains words that have real semantic meaning.
