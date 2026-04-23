Build a recommendation system that, given a user's reading history, predicts what they should read next.

free to define and scope the problem — but be explicit about choices. Some directions to consider:
Recommend the next chapter within all the books a user is currently reading
Recommend a new book to start based on reading history
Handle users or books with little to no history (cold start)

Dataset Overview
You are given two files. 
chapters.csv contains metadata for 50,000 chapters across ~50,000 books — each chapter belongs to a book, has a sequential position within it (chapter_sequence_no), an author, a publication date, and one or more genre tags (pipe-separated). 
interactions.csv contains 1 million records of users engaging with chapters, covering ~150,000 unique users.

chapters are not independent items: they are ordered within a book, and a user's progression through a book carries sequential signals that flat interaction data alone won't capture.
