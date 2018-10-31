# foldercompare

A Windows application that compares the content of two folders from a graphic interface. Outputs a simple report to a .txt file, .csv file, or both. If you're on a Mac or Unix machine, please just use the Bash [`diff`][bash-diff] command.

[Download the program here][exe-download]

For a detailed description of how and why, check out my [blog post][blog]

## Notable Forks

For a more updated version of this program that works with `.zip` files, check out [Juan Biondi's fork](https://github.com/yeyeto2788/foldercompare)

## About

Uses the Python standard library package [`filecmp`][filecmp] to do the comparison and [`tkinter`][tkinter] to build the GUI. [PyInstaller][pyinstaller] is used to package the script into an executable.

## Building the .exe

1. Install [Python 3.5][python]
2. Clone this repo
3. Install requirements using `pip install -r requirements.txt`
4. Run tests using `python -m unittest tests/test_foldercompare.py`
5. Build the program using the script `./build_exe.sh`
6. The standalone program is now located in the top-level folder


[bash-diff]: http://ss64.com/bash/diff.html
[blog]: https://roche.io/2016/06/01/comparing-folders-python
[exe-download]: https://raw.githubusercontent.com/rocheio/foldercompare/master/foldercompare.exe
[filecmp]: https://docs.python.org/3.5/library/filecmp.html
[pyinstaller]: http://www.pyinstaller.org/
[python]: https://www.python.org/downloads/
[tkinter]: https://docs.python.org/3.5/library/tkinter.html
