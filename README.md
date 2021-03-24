# omaralab.github.io

To add a new team member add a file in the folder _staff in the following format

```Liquid
---
name: someone
photo: imagefile
role: role in the lab
quals: graduate awards
rank: 1 = PI, 2=PostDoc, 3=PhD 4=honours 5=undergrad
email: email address
---
# {{page.name}} 
### {{page.quals}}

![{{page.name}}](/images/{{ page.photo }})

* [{{page.email}}](mailto:{{page.name}})

{% comment %}
  Add narrative content here
{% endcomment %}
```  
Add a photo in the /images folder and 
