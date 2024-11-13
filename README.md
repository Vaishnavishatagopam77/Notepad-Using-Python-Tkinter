# Notepad-Using-Python-Tkinter

# Introduction:
tkinter is a GUI library provided by Python to create GUI applications. In this project, with the help of this library, we are going to build up the notepad, a text editor. The notepad will have two main menu items: File & edit. The functionalities of these menu items will also be there.

# Explanation:
First of all, we will import the tkinter library. With this, we will also import the “filedailog” module from tkinter which will provide the classes and factory functions for creating file selection windows.

Now, we will initiate a class named “Notepad ” by using the “class” keyword. During this process, we will pass the parameter as “tk. Tk” which will create the root object for our GUI application. Under this, we will define a “__init__” constructor with self,*args,**kwargs as parameters.

Under this constructor, we will define the title by using “.title” and create a Text widget with the help of the “.Text()” method and will make this widget fill the entire frame with the “.pack()” method.

For the notepad to show the menu bar we will create the menu widget with the help of “.Menu()”.

The functionalities provided by the File menu in this project will be: New, Open, save and exit.

and the functionalities provided by the edit menu will be: cut, copy, and paste

The following options will be created by using the “.add_cascade()” method. This method will create a new hierarchical menu by associating the given menu with the parent menu. While doing so, we will pass the user-defined functions which will carry the particular functionality, under the “command” parameter. By this, both main menu items will get created.

Let’s discuss all the user-defined functions which will be needed to add functionalities to this project.

new_file(): To open the new file. For this, we will clear the content of the text widget by using “.delete()” and then will set the title again as Notepad.
open_file(): To open the existing file. For this, we will make use of the “.askopenfile()” method of the filedialog module to show a dialog that allows a single file selection. After that, it will read the file by the “.read()” method and then give the functionality to insert the data by using the “.insert()” method.
save_file(): To save the file. For this, we will make the save as dialog by using the “.asksaveasfile()” method, then to get the text for further processing will make use of “.get()” and then write the content of the file by using the “.write()” method and then set the title of the text editor with the addition of the file name.
cut(): To remove the text. For this, we will generate a cut event that shows some action and bring the procedure of removal of text into existence by using the “.event_generate(<<event-name>>)” method.
copy(): To copy the text. We will follow the same procedure for generating the event and then will pass the event name which we want to generate as Copy.
paste(): To paste the text. For this as well, we will follow the same procedure for generating the event and name the event Paste
.

In the end, we will call the main method and under this method, we will create the object of the Notepad class named “notepad” and will run the mainloop by using “.mainloop()”.

# OUTPUT: 

![image](https://github.com/user-attachments/assets/cbacb55c-479a-46b3-8caf-36247b28ccff)


By following the above-mentioned procedure, you can create Notepad!
