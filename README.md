# omaralab.github.io

## Adding a new staff member

Add a file in the folder _staff in the following format

```Liquid
---
# this person's full name
name: someone
# file name of a propfile photo for this person
photo: unknown.jpg
# the url this page should be shown on.  Default will be /staff/filename.html
permalink: /someone
# the role for this person that will be shown on the staff page
role: role in the lab
# the academic awards for this person 
quals: graduate awards
# Rank determines the order this person's image will be shown on the staff or emeritus page
rank: 1 = PI, 2=PostDoc, 3=PhD 4=honours 5=undergrad
# fill in this field to show the person's email on this page
email: email address
---
# {{page.name}} 
### {{page.quals}}

![{{page.name}}](/images/{{ page.photo }})

* [{{page.email}}](mailto:{{page.name}})

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
[Some link](https:somelink.com/)
![Some image](/images/unknown.jpg)
```  
Fill in all the field in the *front matter* 
Add a photo in the /images folder and put the file name in the photo field, or select unknown.jpg 
You can copy the file as is to and from the _emeritus folder 
Replace the lipsum text with further markdown content

## Adding a news item
Add a file in the folder _staff in the following format

```Liquid
---
# Enter a title to be shown on the news page
title:  ""
# Date is used to reverse chronologically sort the items
date:   2018-05-18 
# categories are TV, Publications, Awards, Other
categories: Publications
---
# Published 

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
[Some link](https:somelink.com/)
![Some image](/images/unknown.jpg)
``` 

## Adding a new publication item
Add a file in the folder _publications in the following format

```Liquid
---
# Enter a title to be shown on the publish page
title:  ""
# date is used to chronologically sort the items
date: 2018-01-25 
# year is used to chronologically group publications 
year: 2018
# cite is the citation of the publication
cite: ""
# When DOI is provided the entry will have a link
DOI: 10.1371/journal.pone.0191882
# First author used to sort the publications alphabetically 
FI: Condic-Jurkic
---
# Published 

[{{page.cite}}](https://doi.org/{{page.DOI}})
``` 


