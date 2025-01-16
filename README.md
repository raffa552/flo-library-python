## What is flo library?  
Flo library is a Python library that I developed myself.

## What is the purpose?  
The purpose of this library is to make it easier for novice programmers to perform file operations.

## How to install?  
For usage, you can open your terminal and paste the following command:  

```bash
pkg install git
git clone https://github.com/raffa552/flo-library-python.git
cd flo-library-python
pip install flo-1.0.tar.gz
```
## how to use?
to use it in a script must be given
```python
from flo.flo import flo
```
Example script:
Reading a file (JSON, CSV, text, etc.):

```python
from flo.flo import flo
# For reading file
flo.connect('path/to/file')
Writing to a file (JSON, CSV, text, etc.):
```

1. connect(file_path)
This method reads files and returns their content based on file type. Supported formats include .pkl, .json, .txt, and .csv.
Example usage:

```python
from flo.flo import flo
data = flo.connect('path file for read')
print (data)
```
2. write(file_path, data)
This method writes data to the specified file, supporting .pkl, .json, .txt, and .csv.
Example usage:

```python
flo.write('path and file', {"key": "value"})
```
3. unzip(zip_path, extract_to)
Unzips a .zip file to the specified destination.
Example usage:

```python
flo.unzip('archive.zip', 'output_folder')
```
4. zip(output_zip, *paths)
Compresses files or folders into a .zip file.
Example usage:

```python
flo.zip('output.zip', 'folder1', 'folder2')
#can also be used for files
```
5. create(file_path)
Creates an empty file at the specified path.
Example usage:

```python
flo.create('newfile.txt')
```
6. rm(path)
Removes the specified file.
Example usage:

```python
flo.rm('oldfile.txt')
```
7. encrypt(file_path, key)
Encrypts a file using a key. The file is encrypted using the XOR operation and saved as .enc.
Example usage:

Example script
Reading a file (JSON, CSV, text, etc.):

```python
from flo.flo import flo
flo.encrypt('file.txt', 'secretkey')
```
8. decrypt(file_path, key)
Decrypts an encrypted file using the same key.
Example usage:

```python
flo.decrypt('file.txt.enc', 'secretkey')
```
