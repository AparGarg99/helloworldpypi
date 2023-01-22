# Overview
How to build python packages for pip ([pypi](https://pypi.org/)).

# Installation and Usage

1. Create account on [pypi](https://pypi.org/account/register)
2. Open Anaconda command prompt
3. Create new anaconda environment
```
conda create -n "project" python==3.7
```
4. Activate anaconda environment
```
conda activate "project"
```
5. Install the required dependencies for package upload to pypi
```
pip install setuptools twine
```
6. Clone this repository - https://github.com/AparGarg99/helloworldpypi.git
7. Make changes inside `base-folder` (You can choose [License](https://choosealicense.com/), [gitignore](https://www.toptal.com/developers/gitignore/))
8. Navigate to `base-folder`
```
cd ..\base-folder
```
9. Upload package to pypi
```
python setup.py sdist bdist_wheel
```
```
twine upload dist/*
```

# References
* https://www.youtube.com/watch?v=GIF3LaRqgXo
* https://www.youtube.com/watch?v=tEFkHEKypLI&t=9s
* https://github.com/Hritik21/Pypi-Package/blob/main/BUILD%20YOUR%20FIRST%20PYPI%20PACKAGE.pdf