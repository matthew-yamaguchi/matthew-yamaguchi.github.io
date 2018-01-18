---
layout: project
type: project
image: images/ics_211_bst.png
title: ICS 211 - Bookstore
permalink: projects/ICS211_Bookstore
# All dates must be YYYY-MM-DD format!
date: 2017-04-06
labels:
  - Java
  - Data structures
  - Binary search tree
summary: Bookstore that implements a binary search tree
---

<img class="ui image" src="{{ site.baseurl }}/images/ics_211_bst.png">

This project was assigned to our ICS 211 class in the Spring of 2017.  We were tasked with programming the interface for the clerks at a bookstore.  The user needed to be able to stock up on books for the store, sell books, and list all the books in stock.  When the user created a book, they were prompted to enter the title of the book and the ISBN.  After this was successfully completed, the node containing a book object would be added to a binary search tree.

I started by working on the node class and the book class.  After finishing this, I moved onto writing the code for the binary search tree.  This was the most tedious part of the project, as I had to consider all cases where the code may not work as expected.  Some nodes and books were lost in trial and error, but I eventually covered all possible cases.  Next, I programmed the interface for the user, the bookstore class.  In this class, I implemented all the other classes to function based off the user's input.

I felt that this assignment was great for honing my programming skills.  We were required to use all of our prior knowledge of programming to succeed on this assignment.  In addition to this, I also learned a lot about how data structures function.  

