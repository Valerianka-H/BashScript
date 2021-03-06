# script.sh
                             Bash script for finding files in a given directory.

The script takes 2 command line parameters. The first parameter is the name of the directory in which (and in whose subdirectories recursively) to search. The second parameter, which is optional, is the search pattern. If the first parameter is missing, the script outputs a string that describes the correct format for calling the script.  

The script searches the specified directory and its subdirectories for all files whose names match the search pattern. If the template was not specified, then all files except "." and "..". The script generates a list of found files, contains the file name, full path to the file, file type, file size in bytes, and MD5 hash. The list is printed to standard stream.  

The script handles errors such as incorrect file names and search pattern, absence of a specified directory, access errors (in particular, lack of access rights to certain files), absence of any files that match a specified template.
