# Add your own landing page

If you want to modify the project with your own landing page there are two ways to achieve that.

First option is to disable the landing page from the settings page but in that case you will need to install the landing on subdomain/domain and have the system on other location.

![](https://gblobscdn.gitbook.com/assets%2F-MRvYy02Z4zD5OD7PLtd%2F-MYA5EFbwOv2eg3rAQ-J%2F-MYA5iRXCVaFgWV-MAFk%2FScreenshotdsfsdfsd.png?alt=media&token=ce81bbac-bf05-422d-af17-50cd6143cd40)

The second option is to override our default landing page by changing the source code itself.

The landing page is located in **resources &gt; views &gt; social &gt; home.blade.php.**

Open the file and remove all the code inside. Put your HTML code there and save the file.

As usually every landing page have predefined css/js/images files so you will need to put somewhere in the project.

Open the **public** folder and create empty folder and put some name that will define the new landing page location.

Copy all the landing page source code and paste it in the new created folder.

Now open again the file in location resources &gt; views &gt; social &gt; home.blade.php and find all the imports in the **head/script** sections and override to get the files from the new created location.

For example if you have

you need to change it to

After these changes the new landing page should be available.

