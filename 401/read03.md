# reading files in Python

 ## What is a file?

    <br>

    A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.
    <br>

 Files on most modern file systems are composed of three main parts:

  * Header: metadata about the contents of the file (file name, size, type, and so on)
  * Data: contents of the file as written by the creator or editor
  * End of file (EOF): special character that indicates the end of the file

  ## File Paths
  When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

* Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
* File Name: the actual name of the file
* Extension: the end of the file path pre-pended with a period (.) used to indicate the file type