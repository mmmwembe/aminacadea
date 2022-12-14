# Project description
## Aminacadea
### Overview
The Aminacadea library is a dummy helper for tflite-model-maker for use in Google Colab. In Planning phase.

### Requirements
Refer to requirements.txt for dependent libraries that're needed to use the library and run the demo code.
Note that you might also need to install sndfile for Audio tasks. On Debian/Ubuntu, you can do so by sudo apt-get install libsndfile1

### Installation

```python
pip install aminacadea
```

Aminacadea depends on tflite-model-maker >=0.4.2, Pillow >=9.3.0


https://packaging.python.org/en/latest/tutorials/packaging-projects/


#### Generating distribution archives
Generate distribution packages for the package. These are archives that are uploaded to the Python Package Index and can be installed by pip.
NOTE: Run as Adminstrator
1) Make sure you have the latest version of PyPA’s build installed:
```python
python -m pip install --upgrade build
```
2) Now run this command from the same directory where pyproject.toml is located:
```python
python -m build
```
This command should output a lot of text and once completed should generate two files in the dist directory:


#### Uploading the distribution archives

3) To securely upload your project, you’ll need a PyPI API token. 
Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”.

4) Now that you are registered, you can use twine to upload the distribution packages. You’ll need to install Twine:
```python
python -m pip install --upgrade twine
```
   
5) Once installed, run Twine to upload all of the archives under dist:
```python
python -m twine upload --repository testpypi dist/*
```

