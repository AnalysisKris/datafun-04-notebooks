#
#

# Project Information

## Name: 
Kristen Finley 

## Course: 
44-608 Data Analytics Fundamentals 

## Date: 
07February2023 

## Title: 
Module 04: Datafun-04-notebooks

## Assignment Overview
The assignment explores:
- the Jupyter environment and notebooks - a web-based approach that combines code with formatted text and automatic display of results.  
- tools for working with one-dimensional and two-dimensional data.
- the string class and let you know that regular expressions exist to help us identify and parse elements of text (e.g. a phone number or web address).
---
#
# "Datafun-04-Notebooks" Instructions
---
## Chapters
- Read and worked through the Jupyter intro in Ch 1.10.3.
- Read and worked through the book and examples from Chapters 7 and 8.
Focused especially on 7.14.2 pandas DataFrames.
## Additional Reading
- Markdown <https://nwmissouri.instructure.com/courses/50814/pages/markdown?wrap=1>
- Project Jupyter (Official Website)Links to an external site. <https://jupyter.org/>
    - TryLinks to an external site. <https://jupyter.org/try>
    - DocumentationLinks to an external site. <https://docs.jupyter.org/en/latest/>
## Installations
Downloaded and installed some powerful, industry-standard modules for data analytics. 
1. Followed (or confirm you already have followed) the instructions here: https://github.com/denisecase/datafun-01-textbook/blob/main/UPDATED_SETUP.mdLinks to an external site.
2. Read and followed these instructions next: https://github.com/denisecase/datafun-01-textbook/blob/main/RUN_ALL.mdLinks to an external site.
3. Got modules as needed. 
4. Understoond the critical skill-- how to install packages/modules into your standard environment. Noting:
    - If using conda, try to install from the conda-forge channel. 
    - If the module you need isn't available from conda-forge, install it using the pip in your conda module Links to an external site..
    - If you have troubles exporting to HTML, try installing nbconvert.
## Notebooks in VS Code - or Just the Browser?
- Browser: Some analysts work with Jupyter right in their browser. There's more space and we get some benefits of an IDE.
- VS Code: Some analysts work with Jupyter notebooks from within VS Code. On a smaller laptop screen, it can be a bit crowded, but it has benefits. 
- Tried them both -
See <https://nwmissouri.instructure.com/courses/50814/pages/vs-code> for more.


## Start Jupyter
- Once Jupyter has installed into your active environment, started it up by following the instructions in the book Ch 1.10.3:
- In Terminal (Mac) or Anaconda Prompt (Windows), ran jupyter lab. 
For more instructions, see: https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.htmlLinks to an external site.

Got it running both inside VS Code - and without VS Code - so  an informed choice on preference could be made. 
- My preference is VS Code.

## Task 0 - get started
1. Logged in to GitHub account. 
2. Created a new GitHub repo named datafun-04-Notebooks.
3. Git cloned new repo into your Documents folder. 
4. Ensured your repo has the 3 basic files all our repos need:
    - a good README.md,
    - .gitignore, and
    - about.py. 
5. Copied these from previous repos as needed.
6. Updated README.md to reflect the focus of this module. 
7. Added new files to your repo as described below.
8. Git added, git commited, and git pushed (commit/sync in VS Code) your updated content to GitHub.

---
# Task 1 - yourname_1.ipynb
1. Started the Jupyter environment on machine from Documents folder.
2. Used the navigation window to get repo for this module. 
3. In repo, created a new notebook in Jupyter (name the file yourname_1.ipynb), ie. kristenfinley_1.ipynb.
4. Researched how to add Markdown to a Jupyter notebook.
5. At the top of new notebook, changed the first cell from Python to Markdown.
6. Added name as a top-level heading in Markdown at the top of the file
7. In the next cell of notebook, changed back to Python code. 

Used the text, did a search, found a video for getting acquainted with notebooks.

Added a Markdown cell for each section heading.

#### Task 1 - Series 
1. Looked at using a one-dimensional pandas Series to hold and process simple exam data.
2. Followed the instructions in 7.14 to import the pandas module (as pd).
3. Created a pandas Series named grades from a list of integers (exam scores).
4. Got the value of the first grade with grades[0].
5. Called the built in Series functions: count(), mean(), min(), max(), std(), and describe().

#### Task 2 - Series from Dictionary
1. Followed the instructions in the "Dictionary Initializers' subsection to modify your code to initialize grades with a dictionary (a set of key-value pairs instead) - used the student name as the key and their exam score as the value. 
2. Got Eva's score by calling grades['Eva']
3. Got Wally's score using the easier dot notation: grades.Wally.  This is much more common and can be used as long as there are NO spaces in the key text.  If there are spaces, you'll have to use the approach we used for Eva above - wrapping the key in single quotes. 
4. Used the Series values attribute to display the array of values. 
5. Completed the self-check on Page 266. 
6. Noted: We can use a Series whenever our values are a simple one-dimensional array.  
7. Made sure the notebook is nicely formatted with a heading and sections in Markdown clearly dividing the work. 

Ran the entire file and exported the results to kristenfinley_1.html. This displayed the calculated results. 

 ---
# Task 2 - yourname_2.ipynb
1. Read the text Ch 7.14.2.
2. Use a DataFrame, for more complex data. Noted: In a DataFrame, each value is a Series of numbers.
3. Noted: a two-dimensional DataFrame can be used to handle many  exam scores for each key/student.
4. Created a new notebook to practice using DataFrames.
5. Named the notebook kristen_2.ipynb.
6. Used Markdown skills to add a customized title to notebook. 
7. Used Markdown heading for each section below.

## Task 1. Create DataFrame

1. Followed the instructions in 7.14.2 to import pandas as pd and created a pandas DataFrame from a dictionary (a set of key-value pairs) holding multiple exam scores for each key/student. Noted: In this example, there are 5 students, each with 3 exam scores, but the scores aren't labeled.  

## Task 2. Custom Index

1. Followed the instructions to apply a custom index (instead of 0,1,2), called them 'Test1', Test2', and 'Test3'. Saw 'Customizing a DataFrame's Indices with the index Attribute subsection. 
2. Requested grades by key using the text attribute (square brackets with single quoted text strings). Found Eva's grades with grades['Eva'] 
3. Noted: If no spaces in the key, the simpler dot attribute approach can be used. Found Sam's grades with grades.Sam as shown in 'Accessing a DataFrame's columns' subsection. 

## Task 3a. Accessing Rows (loc, iloc)

1. Noted: Like spreadsheets, we can access specific rows or columns.
2. Noted: We use loc['ColA'] and iloc[i]  to access rows by name and index, respectively.
3. Executed the examples using loc['Test1'] to get scores for the first exam, or iLoc[0] to get scores for the first exam and iLoc[1] to get scores for the second exam.
    Answered Question: "Which do you prefer?"
4. Noted: We can also get slices of rows, e.g., from ['Test1':'Test3'], inclusive, or, using index values, from [0:2], inclusive.

## Task 3b. Accessing Subsets (at, iat)

1. Noted: We can use similar notation to get a single cell in the DataFrame (much like getting a single cell in a spreadsheet). 
2. Used grades.at['Test2', 'Eva'} to find her score on the second exam using labels.
3. Used grades.iat[2,0] to get the score on the third exam for the first student (Wally), using indices. 

## Task 4. Describe (By Column)

1. Used grades.describe() to get descriptive statistics for our gradebook columns.
2. Noted that learning Python and DataFrames can be powerful. 
3. Tried to set the precision using the pd.set_option('precision',2) provided.
4. Answered Question. "Does it work?" Noted: Libraries are evolving. If you get an error, copy the error text and do a web search.
    - Error occured. 
    - Google search stated "The following will not work because it matches multiple option names, e.g. display.max_colwidth, display.max_rows, display.max_columns:" 
5. Answered "Can you find something about a newer option using "display.precision"?"
    - source: https://pandas.pydata.org/docs/user_guide/options.html
6. Tried pd.set_option("display.precision",2).
    - Adding "display." before precision corrected error.
7. Noted: Being able to debug evolving features on your own is important for success.
8. Noted: Our field, languages, and libraries are constantly evolving. 

## Task 5. Transpose (rows <--> columns)

1. Got the average for each column by calling grades.mean()
2. Transposed the DataFrame using the T attribute.
3. Got the mean by the new columns with .T.describe()

## Task 6. Sort 

1. Sorted the gradebook rows in reverse order so the most recent exam row appears at the top with grades.sort_index(ascending=False)
2. Sorted the gradebook columns so the names appear in order using grades.sort_index(axis=1).
3. Noted and added examples: We can sort our data pretty much however we like. 

Madesure the notebook was nicely formatted with a heading and sections in Markdown clearly dividing the work. 

Ran the entire file and export the results to yourname_2.html. This will display your calculated results. 

Noted: Minimal submissions earn minimal credit. Repos clearly demonstrating practice, in an organized fashion, with custom notes and remarks are eligible for maximum credit. 

 
---
# Task 3. Push Repo to GitHub
Noted that repo had at least the 3 basic files. 2 notebooks, and 2 exported html files.

Used VS Code to commit and sync (pushed) repo to GitHub - or in Git Bash or terminal, did the following. 

    - git add .
    - git commit -m "added code"
    - git push origin main


---
# Task 4.  Read about String Methods
1. Noted: String methods are helpful for processing text.
2. In 8.9, read "Joining Strings" on page 295 carefully and noted the following:
    1. string.join() is an important and widely used method when working with text. 
    2. The string holds the separator and we pass one argument to the join() method - a list, or a list comprehension.
3. Got an idea of what's possible with strings and string methods. 
4. In 8.11, read about raw strings (with an r instead of an f in front).
5. In 8.12, read about regular expressions - a powerful way to locate specific elements of text (e.g. a phone number). 
6. Noted: We'll do more with strings and text in Web Mining and NLP.
7. Attempted the bonus for more practice.


---
# Task 5. Bonus
1. Noted: Raw data is rarely ready for use.
2. Noted: Data preparation can be about 75% (or more) of our work.
3. Worked through Ch 8.13 to get an idea of wrangling (cleaning & transforming) data.
4. Created an additional notebook named xtra_p4.ipynb.
5. Started by creating the list of contacts in "Reformatting your Data" on page 310.
6. Created a DataFrame. 
7. Noted: The phone numbers are not formatted.
8. Followed the text to create a function that uses regular expressions (usually abbreviated regex or re) to create a function to get a formatted version of the unformatted phone number. 
9. Used map() and your function to improve the DataFrame 
10. Verified phone numbers now appear with two dashes (e.g., 555-555-5555). 
11. Prepared notebook with a nice header (include a title, your name, and date)
12. Clearly labeled steps and result. 
13. Executed the entire notebook, exported it to xtra_p4.html.
14. Commited and push both files into your GitHub repo. 