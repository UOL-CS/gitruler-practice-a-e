<!--
Marked Style: Github
-->

# GitRuler Practice A-E

This repository provides you with practice of all of the git skills you have learned. The topics that are tested in this exercise are:

1. Committing new and existing files
2. Create commits that contains only specific files
3. Ignoring files
4. Finding the status of files in the working directory.
5. Moving and removing files
6. Using the repository log
7. Creating and merging branches
8. Resolving merge conflicts
8. Tagging

## Introduction

In this exercise we'll continue the creation of a book. The book is partly written. Each chapter is a file within the `files\chapters`. To keep track of the plot and characters there are files within the `files\structure` folder.

## Adding the next two chapters

1. Our author has completed writing chapter 5 and started chapter 6 but didn't commit them. Commit chapter 5 with the message "Chapter 5 complete".
2. Finish chapter 6 by adding the final word "headache". Commit that file with the message "Chapter 6 complete".
3. The author started chapter 7 but never committed it. We decided that it's not good. Delete it from the working directory.

## Removing his appendix

Our author thought that factual information at the end of the novel would make it interesting. He added an appendix-a in the chapters folder. Our publisher doesn't like the idea. 

1. Delete appendix-a from git and tell git to ignore all files in the chapter folder that start with appendix. Commit both of these changes with the message 'Ignore appendices'.

## Splitting the book into two volumes

We decide to split the book into 2, so we can sell more books. 

Create new folders so that the structure looks like this:

```
files/
├── books/
│   ├── book-1/
│   │   └──chapters
│   └── book-2/
│       └──chapters
└── structure/
```

Before we make this big change, tag the latest commit with the name "one-volume-version"

Move chapters 1, 2 and 3 into book-1 and chapters 4, 5 and 6 into book-2. Commit all of this with the message "Create two books".

Tag this latest commit with the name "two-volume-version".

## A re-write

The publisher wants to experiment with a more exotic version of the books while the current version is being printed.

1. Create a branch called "exotic".
2. In this branch change `car` to `ice-cream van` in chapter 4.
3. Commit this change with the message "Change book to exotic".

Meanwhile we realise, just before the book is printed, that Grant never learned to drive and so we need to remove references to his car from the book.

1. Back on the master branch, remove the first line (and the following empty line) from the start of chapter 4. Commit this with the message "Remove the car".

Now we're ready to publish the exotic version. 

1. From the master branch merge in the exotic branch.  
2. Oh dear, a merge conflict. Resolve this to keep the line about the ice-cream van. Commit this with the message "Keep Ice-cream".

## Submitting the results

Once the exercise is complete, push this repository to the remote. If there are multiple branches or tags for an exercise, make sure that you push them all. 

To ensure that you have you correctly pushed everything that you need to, you could clone the remote repository into a separate folder and re-run gitruler.
