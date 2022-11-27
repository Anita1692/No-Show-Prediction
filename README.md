# No-Show-Prediction

To run all models we need following datasets which are given in data directory.
* vehicle_data.csv
* Issue Arena.csv
* output.csv
    * To generate this file you need to run NoShow_Part1_Data_Generation.ipynb or you can simply use given output.csv

<b>Installing Graphviz and pydotplus </b>

#### Windows Instructions
* To install graphviz and pydotplus , you need to open the Command Prompt window by  clicking the Start button. Open the Terminal window if you’re using a Mac. In the search box,  type Command Prompt, and then, in the list of results, click Command Prompt. 
    * At the command prompt, type pip install Graphviz. 
    * After Graphviz is installed, type pip install pydotplus.
    * Close the command prompt window. <b>Important </b>: You might have to add the path to the windows system environment PATH: To do  this, go to <b>control panel -> system and security -> system -> advanced system settings - >  environment variables </b>. 
* Click on PATH in the User Variables window, then Edit. 
* Go to the end of the path (it's really long) and add the following: ;C:\Program Files (x86)\Graphviz2.38\bin 

This is the default path for where the graphviz executables are found. If you change the default  installation path when installing graphviz, then you would have to substitute that path for the  one in step 2. You also have to make sure to include the semi-colon in the front of the path. 

<b> MAC Instructions </b>
* To install graphviz and pydotplus , you need to open the Terminal application. To do this, you can also locate the Teminal application using Spotlight.  
    * At the terminal prompt, type pip install Graphviz. 
    * After Graphviz is installed, type pip install pydotplus.  
    * Close the terminal and the environment, and reopen it 
<b> Important: </b> In the example python program, get rid of line 20 (os.chdir("C:\TREES")---it's a PC  command. 

When you read in the data set with the pd.read_csv, just put the full path name in  the quotes inside the parentheses. For example ,open the Applications folder, then open the  Utilities folder and open the Terminal application. 

data = pd.read_csv("/Users/jrose01/Coursera/Machine_Learning /treeaddhealth.csv") 

When you run the programs, you may get an error message that reads “TypeError: string  argument expected, got 'str' “.  
To avoid this, replace the code 
from io import StringIO 
with 
from io import BytesIO as StringIO


<b> Installing PowerBI Dashboard </b>
* To get Power BI Desktop, you can use one of the two approaches.
Install as an app from the Microsoft Store.
Download directly, as an executable you download and install on your computer.
*  Download desktop version from  https://www.microsoft.com/en-us/download/details.aspx?id=58494&WT.mc_id=rss_alldownloads_all
