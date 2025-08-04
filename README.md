# python-project-

i  am going to do the python project
import os

import shutil



def create\_file(filename, content=""):

&nbsp;   with open(filename, 'w') as f:

&nbsp;       f.write(content)

&nbsp;   print(f"Created file: {filename}")



def read\_file(filename):

&nbsp;   if os.path.exists(filename):

&nbsp;       with open(filename, 'r') as f:

&nbsp;           print(f"\\nContents of {filename}:\\n{'-'\*40}")

&nbsp;           print(f.read())

&nbsp;   else:

&nbsp;       print(f"File '{filename}' does not exist.")



def append\_to\_file(filename, content):

&nbsp;   if os.path.exists(filename):

&nbsp;       with open(filename, 'a') as f:

&nbsp;           f.write(content)

&nbsp;       print(f"Appended to file: {filename}")

&nbsp;   else:

&nbsp;       print(f"File '{filename}' does not exist.")



def rename\_file(old\_name, new\_name):

&nbsp;   if os.path.exists(old\_name):

&nbsp;       os.rename(old\_name, new\_name)

&nbsp;       print(f"Renamed file from {old\_name} to {new\_name}")

&nbsp;   else:

&nbsp;       print(f"File '{old\_name}' does not exist.")



def delete\_file(filename):

&nbsp;   if os.path.exists(filename):

&nbsp;       os.remove(filename)

&nbsp;       print(f"Deleted file: {filename}")

&nbsp;   else:

&nbsp;       print(f"File '{filename}' does not exist.")



def list\_files(directory='.'):

&nbsp;   print(f"\\nFiles in directory '{os.path.abspath(directory)}':")

&nbsp;   for item in os.listdir(directory):

&nbsp;       if os.path.isfile(os.path.join(directory, item)):

&nbsp;           print(f" - {item}")



\# --- Sample Usage ---

if \_\_name\_\_ == "\_\_main\_\_":

&nbsp;   file\_name = "sample.txt"

&nbsp;   new\_file\_name = "renamed\_sample.txt"



&nbsp;   create\_file(file\_name, "Hello, this is a test file.\\n")

&nbsp;   read\_file(file\_name)

&nbsp;   append\_to\_file(file\_name, "Adding more content.\\n")

&nbsp;   read\_file(file\_name)

&nbsp;   rename\_file(file\_name, new\_file\_name)

&nbsp;   list\_files()

&nbsp;   delete\_file(new\_file\_name)

&nbsp;   list\_files()



