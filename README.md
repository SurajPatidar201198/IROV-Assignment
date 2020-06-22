# EyeROV ASSIGNMENT

### Problem Statement
#### Task:
You need to create a GUI Application for the above-mentioned requirements. GUI
application should execute the post-processing script written in python. Input arguments
for the python script are given below:
1. Input_path: Path to the post-inspection directory
2. Save_path: Path to the output folder where processed data should be stored.
3. IP_cam: A boolean value (True or False) to select the type of camera
4. Visibility_value : Integer value indicating the water visibility ranging from 1 to 3.
"visibility" : ["1","2", "3"]
5. Method_used: A number from “method1” to "method6" to select the method to
be used for post-processing.

#### The GUI Application should have :
1. One file picker for Input_path
2. Another file picker for Save_path
3. Checkbox for IP_cam
4. A field to take integer input for Visibility_value
5. Dropdown menu to select Method_used. These drop-down menu items are
dependent on Visibility_value. Methods that should be shown on the drop-down
menu for each visibility value is given below:
1 : ["method1","method2","method3"]
2 : ["method4","method5"]
3 : ["method6"]

6. A Progressbar to indicate the progress of the operation
7. One Button named “Execute” to Execute this operation.
8. Another Button named “Terminate” to Execute this operation.
9. A status field to display the status of the operation.

### Frameworks Used :
1) Django
2) Jquery

### Set of Instructions on how to run the application :
Libraries to install before running the application
1) django
2) django-crispy-forms

To install django use command :
#### pip install django

To install crispy forms use command :
#### pip install django-crispy-forms

To locally run the application move to project folder using command line of simple move to folder and press shift+right_click to open powershell and run command :
#### python manage.py runserver

After running this command development server will start at : http://127.0.0.1:8000/ 
copy-paste it on your browser to view the application.

Glimpes of GUI : 
![Screenshot (1222)](https://user-images.githubusercontent.com/42700950/85283041-52835480-b4aa-11ea-99d8-483da3d50180.png)

Ouput that we got after taking entries from the form :
![99999](https://user-images.githubusercontent.com/42700950/85283719-72674800-b4ab-11ea-9c7e-a90861b641c3.PNG)

Yellow shaded potion : First is input path, second is ouput path, third is cam true/false, fourth is visibility value and fifth is method used these are then passed in
backend function defined in views.py of app1.

Some points to take care of :
I have defined backend function in views.py.
