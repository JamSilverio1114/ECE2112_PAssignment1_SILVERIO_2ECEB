# PROGRAMING ASSIGNMENT 1
INTRODUCTION TO PYTHON PROGRAMMING

---

**NAME:** SILVERIO, Jamille Anne &emsp;&emsp;&emsp;&emsp; **DATE SUBMITTED:** Aug. 27, 2025  
**SECTION:** 2ECEB  

---

## I. Intended Learning Outcomes:
1. To identify the basic codes and functions in Python Programming
2. To be able to apply the different codes and functions in creating a Python program

---

## II. Instructions:
Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter
notebook in the dedicated submission bin.

---

### ALPHABET SOUP PROBLEM
Create a function that takes a string and returns a string with its letters
in alphabetical order.

**Example:**
```python
alphabet_soup(“hello”)  ➞ ehllo
alphabet_soup(“hacker”) ➞ acehkr
```
**Implementation (My Work):**
```python
#DEFINE ALPHABET SOUP
def alphabet_soup(word):
    
    #TAKES THE STRING, ARRANGES IT ALPHABETICALLY, THEN RETURNS THEM BACK INTO A SINGLE STRING
    return"".join(sorted(word))

#PRINTS EXAMPLE OUTPUTS
print (alphabet_soup("hello"))
print (alphabet_soup("hacker"))
```
**Code Walkthrough:**
```python
def alphabet_soup(word):
```
* I defined the function ```alphabet_soup``` using the parameter, ```word```, so I can reuse the logic for any input string.
```python
return"".join(sorted(word))
```
* I used ```sorted(word)``` to get the letters in alphabetical order which returns a list of characters.
* Then I used ```return"".join()``` to combine that list back into a single string to return as the result.
* I combined them to a single-line code to make it more clean and concise.
```python
print (alphabet_soup("hello"))
print (alphabet_soup("hacker"))
```
* I used the ```print()``` function to display the output of the code, with ```alphabet_soup()``` as the parameter.
* From the example, I used ```hello``` and ```hacker``` as outputs for the program.

**Conclusion:**  
The program **successfully** displayed the letters of the strings ```hello``` and ```hacker``` in alphabetical order.

---

### EMOTICON PROBLEM
Create a function that changes specific words into emoticons. Given a sentence
as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:
| Word   | Emoticon |
|--------|----------|
| smile  | :)       |
| grin   | :D       |
| sad    | :((      |
| mad    | >:(      | 

<sub>***Table 1***</subr>

**Example:**
```python
emotify(“Make me smile”) ➞ Make me :)
emotify(“I am mad”)      ➞ I am >:(
```
**Implementation (My Work):**
```python
#DEFINE EMOTIFY
def emotify(s):

    #REPLACES THE FIRST PARAMETER TO THE LAST PARAMETER
    s = s.replace("smile", ":)")
    s = s.replace("grin", ":D")
    s = s.replace("sad", ":((")
    s = s.replace("mad", ">:(")
    return s

#PRINTS EXAMPLE OUTPUTS
print (emotify("Make me smile"))
print (emotify("Show me a grin"))
print (emotify("I feel sad"))
print (emotify("I am mad"))
```
**Code Walkthrough:**
```python
def emotify(s):
```
* I defined the function ```emotify``` that takes a sentence ```s```, and returns a transformed sentence.
```python
s = s.replace("smile", ":)")
s = s.replace("grin", ":D")
s = s.replace("sad", ":((")
s = s.replace("mad", ">:(")
return s
```
* I replaced all the words and their corresponding emoticons (See ***Table 1***) using the ```s.replace("old","new")``` function.
* I returned the fully updated string using the ```return s``` function.
```python
print (emotify("Make me smile"))
print (emotify("Show me a grin"))
print (emotify("I feel sad"))
print (emotify("I am mad"))
```
* I used the ```print()``` function to display the output of the code, with ```emotify``` as the parameter.
* From the example and my own sentences, I used each corresponding emoticons to replace their corresponding words in the sentence.
**Conclusion:**  
The program **successfully** displayed the replacements for each ```smile```, ```grin```, ```sad```, and ```mad```.

---

### UNPACKING LIST PROBLEM
Unpack the list into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

**Example:**
```
lst = [1, 2, 3, 4, 5, 6]
Output:   first: 1   middle: [2, 3, 4, 5]   last: 6
```
**Implementation (My Work):**
```python
#DEFINE LST
lst = [1, 2, 3, 4, 5, 6]

#ASSIGNS THE FIRST VALUE OF THE LIST LOCATED AT INDEX 0
first = (lst[0])
#ASSIGNS THE MIDDLE VALUES OF THE LIST STARTING FROM INDEX 1 UP TO (BUT NOT INCLUDING) -1
middle = (lst[1:-1])
#ASSIGNS THE LAST VALUE OF THE LIST LOCATED AT INDEX -1
last = (lst[-1])

#PRINTS EXAMPLE OUTPUTS
print ("first:", first, "middle:", middle, "last:", last)
```
**Code Walkthrough:**
```python
lst = [1, 2, 3, 4, 5, 6]
```
* I created a list using the example provided, named ```lst```.
```python
first = (lst[0])
```
* I used indexing at ```0``` to get the first item of the list and store it in ```first```.
```python
middle = (lst[1:-1])
```
* I used slicing from index ```1``` up to (but not including) index ```-1``` to get all the middle values.
```python
last = (lst[-1])
```
* I used index ```-1``` to select the last item in the list.
* I did not use index ```5``` as the last parameter so as to always capture the last item in the list in the case that a value will be added at the end of the list. This applies to the ```middle = []``` function.
```python
print ("first:", first, "middle:", middle, "last:", last)
```
* I used the ```print()``` function to display all three variables, ```first```, ```middle```, and ```last``` and their corresponding values.

**Conclusion:**  
The program **successfully** displayed the three variables, showing the ```first```, ```middle```, and ```last``` values on the list ```lst```.

---

**Click here to see my Jupyter Notebook:**  [SILVERIO_2ECEB_PA1.ipynb](https://github.com/JamSilverio1114/ECE2112_PAssignment1_SILVERIO_2ECEB/blob/main/SILVERIO_2ECEB_PA1.ipynb)  
**DATE DUE:** Aug. 27, 2025  

**Updates made on the code:**
* In #3 Unpacking List Problem, the typo in the comment ```#DEINE LST``` was fixed to ```#DEFINE LST```.

---
