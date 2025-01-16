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
### example script 
```python
from flo.flo import flo
#for read file
flo.connect('path and file')
```
```python
from flo.flo import flo
#for whrite file
flo.whrite('path and file', 'text for whrite to file')
```
