# mascot_online
<h1><B>README<B><h1>
Introduction
This project is about opening a .txt file and converting it into a table, then saving it to a .csv file.

Requirements
pandas
json
csv
os
Python Packages and Functions Used
pandas: used to create dataframes and concatenate them
json: used to load the data from the .txt file into a dictionary
csv: used to write the data from the dataframe into a .csv file
os: used to create an absolute path to the .txt file
Code Explanation
The code contains two functions: create_dataframe and write_csv.

create_dataframe function
The function takes two inputs, file_name and df_fct, where file_name is the name of the .txt file and df_fct is the existing dataframe. The function loads the data from the .txt file using json.load and creates a new dataframe from the data. Then, it extracts specific columns from the dataframe, creates new columns based on the values of the 'Attributes' column, drops the 'Attributes' column, and appends the new dataframe to the existing one. The new dataframe is returned.

write_csv function
The function takes one input, df_fct, which is the dataframe that will be written into a .csv file. The function creates a new .csv file using csv.writer and writes the data from the dataframe into the file.
