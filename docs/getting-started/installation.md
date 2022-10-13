---
layout: page
menubar: docs_menu
title: Installation
subtitle: Getting Started
show_sidebar: false
toc: true
---

## Local Installation
1. Clone the [UNAGI repository](https://github.com/Karlxy0511/IPF_Dashboard) and open it
```
git clone https://github.com/Karlxy0511/IPF_Dashboard.git
cd IPF_Dashboard
```
2. Optimially, set up a virtual enviroment to avoid package version conflicts between different projects
on your machine. In this case, we call it `env`:
   1. For mac:
    ```
    python3 -m venv env
    source env/bin/activate
    ```
   2. For windows:
    ```
    python -m venv env
    env\Scripts\activate
    ```
3. Make sure the base interpreter is set to Python3.9. Install the correct version of the necessary packages. Windows users should replace 'pip3' with 'pip':
```
pip3 install -r requirements.txt
```
4. Place the h5ad database on the same level with the `\assets` directory.

5. Run setup.sh
```
chmod u+x setup/setup.sh
./setup/setup.sh dataset_06_22_22.h5ad
```
If you are unable to run setup.sh on your machine, please do the following:
- Create a folder in the same directory called `stage-dataset` by running `mkdir stage-dataset`; this will be gitignored
- Run the segmentation script (replace 'python3' with 'python' if you are a windows user) 
   ```
   cd setup
   python3 segmentation.py --data ../dataset_06_22_22.h5ad --seg stages
   cd ..
   ```

6. Run UNAGI. UNAGI.py requires arguments for both the dataset and iDrem paths. For our current iteration it is (replace 'python3' with 'python' if you are a windows user) :
```
python3 UNAGI.py --data dataset_06_22_22.h5ad --idrem assets/idrem
```
7. Wait for about 3 minutes till a text message shows on your terminal. You can now visit UNAGI at [localhost:8050/unagi](localhost:8050/unagi) on your web browser.

## Usage
In order to successfully run the file you need the `\assets` directory as well as the h5ad database in the same folder as the file.
Add all extrenous `.css` files to assets. 