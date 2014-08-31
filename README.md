at-core-router
==============
at-core-router provides convention based, configuration free view routing.

Views are Polymer web components. The views are loaded to the main section of the at-app-scaffold. 

The router uses the hash of the Url 
folder/page.html#!viewname            - loads viewname.html from the folder where page.html resides
folder/page.html#!component/viewname  - loads viewname.html from ../components/

Parameters can be appended to after a ? in the hash e.g. 
folder/page.html#!component/viewname?arg1=val1,arg2=abc

These arguments are automatically bound to published variables of the view component. 
So if a view publishes an argument arg1 the value val1 is automatically assigned to that argument.

The binding is bidirectional so if the value in the component changes that Url is auto updated as well as if the Url arg1= changes then the attribute value of the view web component is also auto updated.

