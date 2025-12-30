this is simple and small, 
this has no lifecycle safety, 
every time the lifecycle ends > reload, 
but the webp files are small, so it compensates a little


How to set up:

Firstly upload;
news1.webp
news2.webp
1.html
2.html
to your Github repository.

then, you should add the id's and drawable of the image views
you need 2 normal id's,
and 1 drawable id

Name them:
id/news1
id/news2
drawable/newsloading -> this is a placeholder

and then copy the content of YourFragment.xml to your target fragment layout

then copy the id/ and fill them in the smali class YourFragment

then adapt the class names to your app, 
keep in mind YourFragment is only the part you have to add, 
not the whole thing

the classes News$3 and News$4 are click listeners, 
put your target link in them, 
and make sure they point to 1.html and 2.html, so it's dynamic as well

info:
if you will use .webp files as adviced, 
the load time is around 300ms,
depends on the internet quality but 200-300kb shouldn't be a big issue
