---
title: Home
layout: page
menubar: docs_menu
description: "UNAGI is a dashboard that visualizes dynamic single-cell omics data found in the IPF Research."
show_sidebar: false
---

# UNAGI Documentation

**UNAGI** is a dashboard that visualizes dynamic single-cell omics data found in the IPF Research of Yumin Zheng and Dr. Jun Ding of the Meakins-Christie Laboratories at McGill University. UNAGI is built in Python using the Dash framework and relies on several open-source packages.

UNAGI is developed and actively maintained by [the Ding Lab](https://junding.lab.mcgill.ca/) at McGill University.{: .fs-6 .fw-300}

[Visit UNAGI](http://dinglab.rimuhc.ca/unagi/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/Karlxy0511/IPF_Dashboard){: .btn .fs-5 .mb-4 .mb-md-0 }

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

## Core Dependencies
1. H5AD Database: `adataset_06_22_22.h5ad`
2. iDREM: `25/04/2022`
3. Dash Plotly: `dash==2.5.1`
4. Gene dependency:`pathway_genes_in_IPF_dataset.npy`
5. Pertubation dependency:`MAY14_8_markers.npy`
6. `compound_all_target_merged.npy`


## Notes
* https://www.nature.com/articles/s41598-018-28948-z#Sec1
* http://www.cs.cmu.edu/~jund/idrem_lung/
* https://lungmap.net/idrem/index.html
* https://toppgene.cchmc.org/CheckInput.action?query=TOPPFUN&type=HGNC_SYNONYMS&training_set=



## Links
* UNAGI Web Server: http://dinglab.rimuhc.ca/unagi/
* Official Source Code Repository: https://github.com/Karlxy0511/IPF_Dashboard
