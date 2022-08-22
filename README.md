# MADS-Capstone-
# Effect of a cell phone ban on school test scores in Michigan 

<img width="528" alt="image" src="https://user-images.githubusercontent.com/55987309/185806732-8d48438a-fd98-4c36-a416-ebac15db1e3f.png">

This project considers whether a causal relationship exists between banning cell phones in Michigan public school districts and students' academic scores on standardized math tests. We used the Synthetic Control Method to analyze the impact cell phone bans had on student achievement. 

The SyntheticControlMethods package used in our code requires SciPy 1.4.1 which most likely is a downgrade for most users and requires the kernel to be restarted after the install. The pip install is in the first cell of the 4_Cell_Phone_Ban.ipynb notebook. Users can run the install, restart the kernel, and then proceed with the second cell which verifies that scipy 1.4.1 is the current version.

The Census Data API is another specialized package that requires a Pip install and a verification key. The key has been requested and is already embedded in the code. The code functions at the time of this writing.

## Packages

* Pip install SyntheticControlMethods
* Pip install scipy==1.4.1
* Pip install Census Data API

The code is contained in 3 Jupyter notebooks and needs to be run in this order: 
* 2_ACS_Demographic_Data.ipynb
* 3_Clean_MI_Academic_Data.ipynb
* 4_Cell_Phone_Ban.ipynb. 

The code should produce several charts including this one which demonstrates the difference between the school district with a cell phone ban and the synthetic control group which did not institute a cell phone ban.

<img width="1196" alt="image" src="https://user-images.githubusercontent.com/55987309/186026354-f2e0ea19-30b8-48c2-95a5-a5fb81e3a915.png">

The data that the code accesses is contained in the 1_CSV_Data folder. The Michigan school district data came from the [MI School Data](https://www.mischooldata.org/k-12-data-files/) site run by the State of Michigan. The data from the American Community Survey is generator within the 2_ACS_Demographic_Data.ipynb notebook. 
