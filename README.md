# DSpace
Additions of DSPACE API

Below are 2 useful functions I added to the DSPACE API:

1)GET /keywords/{word}
This function retrieves all the distinct values of the metadata field 'word'. 
'word' represents the metadata field name. word is dc.subject. The function will split 'word' by (.) and return all the metadata values
where the metadata field is dc.subject.

Example of call: /keywords/dc.subject

2) POST /
This function does the same thing as (1) but is in the form of a post.


How to use: You need to place these functions in the ItemsResource.java source file. OR
you can use dspace overlays. 
