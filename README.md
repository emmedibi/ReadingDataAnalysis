# ReadingDataAnalysis
An analysis of my reading data exported from [Goodreads](https://www.goodreads.com/).

# Setup
The language used for this analysis is *Python*
## Python and packages used
- Data Manipulation: `pandas` and `numpy`
- Visualization: `seaborn` and `matplotlib`


# Data Source
The file (goodreads_library.csv) is my reading data exported from goodreads.
## Inside the file
The file is composed of the following columns:
- Book Id
- Title
- Author
- Author l-f: author's name in "last name - first name" format
- Additional Authors: if the book has more than one author
- ISBN: International Standard Book Number (for books published before 2007, ISBN has 10 cyphers)
- ISBN13: International Standard Book Number 13 cyphers
- My Rating: value 1-5
- Average Rating
- Publisher
- Binding: kind of bookbinding
- Number of Pages
- Year Published: publication's year of this specific version of the book
- Original Publication Year: the first publication's year
- Date Read: the date where you ended reading the book
- Date Added: the date where you add this book on your shelf
- Bookshelves
- Bookshelves with positions
- Exclusive Shelf
- My Review
- Spoiler: mark if your review has spoiler (true/false)
- Private Notes
- Read Count: how many time you have read the book
- Owned Copies

# Questions
1. How many books I have read from 2019? (from the first year I effectivly used the app)
2. What is the longest book I have read from 2019? And the shorter?
3. Who is the *author* whose books I have read the most?
4.  Who is the *publisher* whose books I have read the most?
5.  The book that waited the least to be read
6.  The book that waited the most to be read
7.  Who is the author whose books I want to read the most in the future?
8.  What is the this year's books I rated 5 stars?
9.  What's my rating average?
10.  What's the relationship between my ratings and goodreads community's ratings?

# Plots
1. the books read per year
2. the books added on my goodreads whishlist per year
3. show the previous two dataset in one plot

# Results and evalutations
From the data I could see that, from 2019, I read 192 books, with this distribution:
![image](https://github.com/emmedibi/ReadingDataAnalysis/assets/55384897/c0eed7f6-5855-4ff1-99bd-c6770ddbacc5)

As you can see, in 2022 (on going) I read more than I did in 2021.

I found out that the author whose books I read the most are comics artist. The publisher I read the most is Longanesi (italian publisher).

I analyze the relationship (correlation) between my ratings and the average of ratings on goodreads.
As you can see from the graphic, the correlation is just above the zero (0,33)
To have the right measure of the correlation, I detected possibile outliers and I dropped them from the datasets.
At the end, the correlation without outliers is closer to zero than the previous one (0,3).

![image](https://github.com/emmedibi/ReadingDataAnalysis/assets/55384897/9806a70e-ec54-4f26-9e08-c3677abc6202)

That means I can't rely on goodreads' average ratings to choose a new book to read.
