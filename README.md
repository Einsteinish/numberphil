#NumberPhil (http://numberphil.com)
----

##Version 1 features

+ Users can share any link of interesting blog post or video in the Resource Section.
+ Resources are divided in topics.
+ Users can share snippets(a shorte blog post) on their wall to share their views and experiences in learning.
+ Users can save interesting resources to their profile for later use.
+ Topic follow button allow users to follow topics to get interesting news, new resources.
+ Explore section lets view the ongoing activity of the site at a glance.

##Later features

+ Moderators and more active users will be able to edit wiki like content in the topics and resources.
+ Tracks will be introduced to give users ability to create content for the their audiences and distribute them.
+ Users can follow other interesting users.


##Tools/Apps Used

+ [Django 1.8.7](https://www.djangoproject.com/)
+ [Twitter Bootstrap](http://getbootstrap.com/)
+ [django-registration](https://django-registration.readthedocs.org/en/latest/)
+ [django-guardian](https://github.com/lukaszb/django-guardian)
+ [django-braces](https://github.com/brack3t/django-braces/)
+ [django-ratings](https://github.com/dcramer/django-ratings/)
+ MySQL (sqlite3 for dev)
+ [django-haystack](http://haystacksearch.org/)
+ [elasticsearch](http://elasticsearch.org/) : sudo systemctl start elasticsearch (run), sudo systemctl enable elasticsearch (booting time autorun)

*For full requirements, see requirment.txt*


##Install

+ See INSTALL.md for full installation instructions.
+ http://www.numberphil.com


## Contact

+ [mail us](mailto:contact.numberphil@gmail.com).

## LICENSE

This project is licensed under [MIT License](http://mit-license.org). See LICENSE.txt

## Note

+ djangoratings-vote : ip-address width = 64. Otherwise, we get the following error: Data truncated for column 'ip_address' at row 1
+ discus comment tool requires registration. 
+ Upgraded to Django 1.8.7 on Jan. 2, 2016 (2 fixes - 1. Import user after loading app, 2. NoReverseMatch for admin delete)
+ Added thumbnail field to resources (resources/models.py)
+ Bug fix for resource image upload by adding enctype="multipart/form-data" to templates/resources/resource_form.html
+ The upload_to folder switched to MEDIA_ROOT/topics/%Y/%m/%d/ and MEDIA_ROOT/resources/%Y/%m/%d/ to resources/models.py to Topic and Resource classes on Jan. 12, 2016.
+ Can use markdown (django-markdown-duex) for TextField such as Description and Help_Text in Resources/Topic. Basic tutorial is available at https://daringfireball.net/projects/markdown/basics.
+ Added a video field as well as a filed for embedded YouTube video to Resources.
+ [Related Tutorials - Deploy numberphil.com](http://www.bogotobogo.com/python/Django/Python_Django_tutorial_Numberphil_Deploy.php)


