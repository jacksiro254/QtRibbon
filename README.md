# QtRibbon
The Ribbon style menu bar implemented by Qt, the basic idea is to customize QTabWidget and adjust the display style through QSS (style sheet). The principle of QRibbon is to try not to invade the development of normal business logic, so when developing programs based on QMainWindow, you can follow The normal development process creates an interface, creates a common menu bar and menu items and their signal slot associations, and finally calls the QRibbon::install(&amp;mainWindow) function to automatically create a Ribbon corresponding to the original QMenuBar of QMainWindow...

## Instructions
* Create QMainWindow normally
* Add menus and menu items to QMainWindow (it is recommended to add appropriate icons for all menu items, so that finally QRibbon can directly use the icon of the menu item as the button icon)
* Add all files related to the QRibbon library to the project
* After the main interface is constructed, the QRibbon can be added by calling the following code:  

    ```QRibbon::install(&mainWindow);```

## Use QtRibbon::install(window) before and after effect comparison
![image](https://github.com/gnibuoz/QRibbon/blob/master/images/QRibbon.gif)

## Use QtRibbon front interface effect
![image](https://github.com/gnibuoz/QRibbon/blob/master/images/%E4%BD%BF%E7%94%A8QRibbon%E5%89%8D.png)

## Interface effect after using QtRibbon
![image](https://github.com/gnibuoz/QRibbon/blob/master/images/Qt-Ribbon.gif)
