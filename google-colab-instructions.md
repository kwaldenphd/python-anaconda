# Getting Started with Google Colab

In case any of you is facing any trouble with installation of or working with Anaconda, fear not. Google Colaboratory (or more colloqially, Google Colab) has got your back. It is quite similar to Jupter notebook with some minor differences (but trust me, those are obviously not going to bother you at all). 


# Goals

By going through this documentation, you will be able to:
- Understand how to add Google Colab app to your Google Drive
- Understand how to create a new Google Colab notebook
- Understand how to change runtime type
- Understand how to mount your Google Drive to your notebooks
- Understand how to create new cells inside the notebook
- Understand how to download the notebook to your local PC


# Table of Contents

- [Add Google Colab App To Your Google Drive](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#add-google-colab-app-to-your-google-drive)
- [Create A New Google Colab Notebook](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#create-a-new-google-colab-notebook)
- [Change the Runtime Type](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#change-the-runtime-type)
- [Mount Your Google Drive To Your Notebook](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#mount-your-google-drive-to-your-notebook)
- [Add New Cells To Your Notebook](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#add-new-cells-to-your-notebook)
- [Download Your Notebook](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#download-your-notebook)
- [Last Few Words](https://github.com/kwaldenphd/python-refresh/blob/main/google-colab-instructions.md#last-few-words)


# Add Google Colab App To Your Google Drive

1. If you have already opened the Gmail app using yourNetID@nd.edu, then left-click on the 9 dots close to the top-right corner and choose "Drive" from the options which appear. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic001.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic001.png?raw=true" /></a></p>

2. Google Drive will open.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic002.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic002.png?raw=true" /></a></p>

3. Now open a new tab in your web browser, go to https://www.google.com, type Google Colab in the search box and hit Enter from the keyboard.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic003.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic003.png?raw=true" /></a></p>

4. Left-click on the first link which appears. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic004.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic004.png?raw=true" /></a></p>

5. Google Colab will open with an additional window on top of it. Just left-click on "CANCEL" on that window.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic005.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic005.png?raw=true" /></a></p>

6. Left-click on "File" and then on "New notebook". A new notebook will open in a new tab but you don’t have to do anything else in that notebook. You may close that tab as it is of no use to us.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic006.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic006.png?raw=true" /></a></p>

7. Return to the tab displaying your Google Drive account and left-click on the Refresh button. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic007.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic007.png?raw=true" /></a></p>

8. Google Colaboratory is now added to the list of your Google Drive apps. Left-click on "New" → "More" and you would get to see the "Google Colaboratory" app.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic008.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic008.png?raw=true" /></a></p>


# Create A New Google Colab Notebook

9. Create a new folder by left-clicking on "New" → "Folder". 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic009.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic009.png?raw=true" /></a></p>

10. Give a name to the folder --- for example, `EoC_002`. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic010.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic010.png?raw=true" /></a></p>

11. Left-click on "Create" and a new folder will be created. 

12. Inside that newly-created folder, left-click on "New" → "More" → "Google Colaboratory". A new Google Colab notebook will be created. 

13. When you are inside a new Google Colab notebook, you shall get to see 3 main components in the user interface (here lies that `minor difference` compared to the UI of Jupyter notebook)
- Notebook Name
- Menu Bar
- Code Cell

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic011.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic011.png?raw=true" /></a></p>

14. The Notebook Name is what the .ipynb file will be saved as.


# Change the Runtime Type

15. You need to change the runtime type, so that cells can be executed without any interruptions. 

16. In the Menu Bar, left-click on "Runtime" → "Change runtime type". 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic012.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic012.png?raw=true" /></a></p>

17. Next, change the "Hardware accelerator" from "None" to "GPU". Left-click on "Save".

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic013.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic013.png?raw=true" /></a></p>

18. The Runtime Type is now changed for that notebook. Please remember to change the Runtime Type for every notebook you create and work with. 


# Mount Your Google Drive To Your Notebook

19. Type the following code inside the first, blank Code Cell in the Google Colab notebook. 

```Python
from google.colab import drive 
drive.mount('/content/drive')

import sys
sys.path.append('/content/drive/My Drive/EoC_002')
```

20. Please note that, `EoC_002` is the name of the newly-created folder. If your newly-created folder’s name is different, put in that name instead of `EoC_002`.

21. Now, left-click on "Connect" in order to connect your notebook to the Google server.  

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic015.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic015.png?raw=true" /></a></p>

22. Once connected, it would show a green check right next to the texts "RAM" and "Disk". 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic016.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic016.png?raw=true" /></a></p>

23. Now, left-click on the Play button to the left of the Code Cell. Upon doing so, a url will be generated.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic017.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic017.png?raw=true" /></a></p>

24. Left-clicking on that url will take you to the account choosing page. Left-click on the account which shows your ND mail in the following format --- yourNetID@nd.edu. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic018.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic018.png?raw=true" /></a></p>

25. Google Drive will now want to access your account. Left-click on "Allow".

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic019.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic019.png?raw=true" /></a></p>

26. Once it shows a code, copy the code. Please keep in mind that the code is unique for everyone as well as it changes every time you try to mount your drive. Hence, it will be different from the one depicted in the figure below. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic020.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic020.png?raw=true" /></a></p>

27. Now, return to the tab displaying your Google Colab notebook. Paste (Ctrl + v from keyboard on Windows and Linux or Cmd + v from keyboard on MacOS) the copied code into the vacant box right underneath "Enter your authorization code" and hit Enter from your keyboard. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic021.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic021.png?raw=true" /></a></p>

28. If everything is in order, your drive will now be mounted. Please remember to mount your Google Drive every time you create a new notebook. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic022.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic022.png?raw=true" /></a></p>


# Add New Cells To Your Notebook

29. You may want to add new Code Cells (while you are working with codes) or Text Cells (if you want to elaborately describe what you are doing) to your notebook. 

30. In order to add another Code Cell, simply left-click on "+ Code". A new Code Cell will be added right underneath your latest cell. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic023.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic023.png?raw=true" /></a></p>

31. In order to add a Text Cell, simply left-click on "+ Text". A new Text Cell will appear right underneath your latest cell. Note that Text Cells are equivalent to Markdown Cells in Jupyter notebooks. 

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic024.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic024.png?raw=true" /></a></p>

32. Do not forget to save your Google Colab notebook. Save it as and when you deem it necessary and as many times as possible. Periodic saving of your notebook is highly recommended. 


# Download Your Notebook

33. You can download your Google Colab notebook as .ipynb by left-clicking on "File" → "Download .ipynb".

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic025.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/pic025.png?raw=true" /></a></p>

34. Select the location where you would like to save the notebook in your local PC and left-click on "Save". Please double-check that the extension of the to-be-downloaded file is `.ipynb`. Your Google Colab notebook will now be saved as a .ipynb file in your local PC. 


# Last Few Words

35. If you face any problem with Google Colab, please feel free to pose such questions on Slack. We would be happy to answer all your questions. 

36. And finally, hope you have fun working with Google Colab notebook as much as we do and have had in the recent past. Welcome to the course and happy coding! 


