# WpfFolderBrowser
Fork from https://wpffolderbrowser.codeplex.com/

# Project Description
Use the Windows Vista / Windows 7 Folder Browser Dialog from your WPF projects, without any additional dependencies.

# Remarks

This project was adapted from the Vista Bridge sample on MSDN http://msdn2.microsoft.com/en-us/library/ms756482.aspx. Basically, I did only the following:

* Get the example to run under .Net 4.0 .
* Add the FOS_PICKFOLDER option to the initialization code of the OpenFileDialog.
* Add members to set an initial folder and to set the initial text of the file name TextBox.
* Remove members that did not apply to the FolderBrowser dialog.
* Remove unused code and dependencies.
* Rename public classes and namespaces.

As a result, the WPFFolderBrowserDialog class can now be used out of the box in WPF projects, much like the Microsoft.Win32.OpenFileDialog class, which actually lacks only a way to set the FOS_PICKFOLDER option in order to support this scenario (I still hope that some day some one will add this possibility and make this project obsolete!).

Actually, everybody could do this by themselves, but since it took me roughly a day to figure out how to do it, I thought I'd share the result with the community...