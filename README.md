# mascot_online
<h><B>README<B></h>

  
<h1><B>Introduction</h1><B>
  
This project is about opening a .txt file and converting it into a table, then saving it to a .csv file.

<h1><B>Requirements</h1><B> <br>
<p> pandas <br>
json <br>
csv <br>
os <br>
</p><br><br>
<h1><B>Python Packages and Functions Used</h1><B> <br>

pandas: used to create dataframes and concatenate them <br>
json: used to load the data from the .txt file into a dictionary <br>
csv: used to write the data from the dataframe into a .csv file<br>
os: used to create an absolute path to the .txt file<br><br>
  
<h1><B>Code Explanation</h1><B> <br>

The code contains three functions: create_dataframe function, write_csv function (bonus : create_dataframe_folder function)<br><br>

<li><h2><B>create_dataframe() function</h2><B> <br>
  
The function takes two inputs, file_name and df_fct, where file_name is the name of the .txt file and df_fct is the existing dataframe. The function loads the data from the .txt file using json.load and creates a new dataframe from the data. Then, it extracts specific columns from the dataframe, creates new columns based on the values of the 'Attributes' column, drops the 'Attributes' column, and appends the new dataframe to the existing one. The new dataframe is returned.<br><br>

<li><h2><B>write_csv() function</h2><B> <br>
  
The function takes one input, df_fct, which is the dataframe that will be written into a .csv file. The function creates a new .csv file using csv.writer and writes the data from the dataframe into the file.<br><br>
  
<li><h2><B>"create_dataframe_folder() function"</h2><B> <br>
  
 Same as create_dataframe functions adapted for multiple json files as input, it will add multiple row on the dataframe<br><br>
  
<h2><B> Other functions</h2><B> <br>
  
 <li>os: The os package is used to interface with the underlying operating system and perform various tasks related to the file system, such as creating an absolute path to a file.<br><br>

<li>os.path.abspath(): This function returns the absolute path of a file. In the code, the function is used to create an absolute path to the channel_advisor_api_data.txt file.<br><br>

<li>pandas (pd): This is a powerful and easy-to-use data analysis and manipulation library for Python. In this code, the pandas package is used to create dataframes and perform operations on the data.<br><br>

<li>pd.DataFrame(): This function creates an empty dataframe. In the code, it is used to create an empty dataframe called df at the beginning.<br><br>

<li>json: The json package provides functions for encoding and decoding JSON data. In this code, the json.load() function is used to open and load the contents of a json file.<br><br>

<li>json.load(): This function loads the contents of a json file into a Python object. In the code, the function is used to open the channel_advisor_api_data.txt file and load its contents into a Python object called data.<br><br>

<li> drop(): This function is used to remove a column from a dataframe. In the code, the function is used to remove the Attributes column from the dataframe.<br><br>

<li>pd.concat(): This function is used to concatenate two dataframes. In the code, the function is used to append the new dataframe to the existing one.<br><br>

<li>glob: The glob package provides a function for making file lists from directory wildcard searches. In this code, the glob.glob("*.txt") function is used to find all the .txt files in a folder<br><br>
