ALIENS ON EARTH
=====================
Developed this console based application in Java

Main class:  AlienPath.java
  
  My Approach
  ------------
  
1) On loading this application default export formats & Alien secret formats are loaded
2) Alien should  give inputs only in numbers
3) Alien has to give inputs for Main menu
Main menu
---------------
1) New Registration
2) Supported Export Formats
3) Help
4) Exit

4) In New Registration  Alien has to provide their information like

Code Name
Blood Color
No of Antennas
No of Legs
Home Planet

5) Now a bean class has been created , it gets all  information about Alien & export data based on the user selected format (TXT/CSV)

6) In Supported format (option 2) default format that the application supports will be printed. User can select any of them.

PART B
----------------
For registering a new export plugin

Copy your plugin .class file to plugin folder inside user’s home (/home/user/Aliens/Plugins in Linux , C:\users\Aliens\Plugins in Windows)  and restart the application

Your class should implement the ExportService interface, get the interface file from plugin folder of user’s home


Your plugin should have a default constructor, and should be in default package/no package If not, the plugin will not be registered with the system and system can crash


Your class must return the format name using getFormatName method and export data to file using exportData method


Example:     1) Create a Java file (Ex: CsvExportService.java) in default package that should implement 2 methods of interface ExportServices.

             2)  Copy class file newly created Java file & put it in Plugin folder, plugin folder is created automatically when application loads inside user’s home (/home/user/Aliens/Plugins). When application loads new format also loaded. 




                         **********======================================******


       

