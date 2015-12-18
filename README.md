#web.ts
Create Web Apps the Object Oriented way.
An Easier, faster, and efficient way to create websites. 

* For pages, you create a ts class file that extends web.ts.Page.

* For lists, create a ts class that extends web.ts.List<T>. 


##Pages
1. Implement the View() Method to return the location of the view page you would like to show, for example, "/Page1.txt".
You can also return #element (id of an element), which returns the outerHTML content of an element in the document page. The View source file can be designed with HTML Designer softwares.
You can use the View() Method to prepare the document before View(), it will be used once internally.

2. Implement the Render(document) method callback which is used to render the content when it's already available.

3. create instance of this class and call Load() method to ask to fethch the document in View() and Render(doc) when it's finished fetching.

4. Pages are loaded when a Url change is detected and load a different page based on the name of the Hash. 

##List
1. Implement the Add() and Remove() Method to be used in adding or removeing items. And implement View() method to return the document that will be used in rendering.
List class uses Load() and Render() of the page extension internally and the methods, in addition to View() behave the same as Page class.

2. Create an Instance of the class and call List(arr:T) to start the process.