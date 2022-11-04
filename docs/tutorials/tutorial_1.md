---
layout: page
menubar: docs_menu
title: Tutorial - Basic Analysis Pipeline
subtitle: Tutorials
show_sidebar: false
toc: true
---
Tutorial - Basic Analysis Pipeline
---
This is a step by step demonstration of the basic functionalities of UNAGI.

UNAGI accepts .h5ad files and uses AnnData data structure for storing and analyzing. 
<img src="../images/overview_1.png" class="center"/>


UNAGI can be viewed as two parts: two panels on the left side for clusters and genes selection and five tabs 
on the right side for results presentation. We are at the graph tab upon initialization. Inside graph tab, we have a
2D visualization of the tracks and a scatter plot colored by cluster types. The default coloring type of the scatter
plot is cluster, but we can use the dropdown menu to select different coloring options.
<img src="../images/cluster_2.png" class="center"/>

In the 2D visualization graph, each dot represents a cluster and each column represents a stage. We can click the dots
to view the gene expression of that cluster. The results are usually shown in 2s.
<img src="../images/track_1.png" class="center"/>

We can also select the track we want to analyze in the dynamics panel on the left.
If a control cluster is selected, the clusters for different stages will be automatically filled in. 
Once you have selected a track, click "Confirm Track" to confirm. After this, the scatter plot will be reloaded and
show the results of the selected clusters in a few seconds.
<img src="../images/dyna_2.jpeg" class="center"/>

We can also click the "3D" button in the dynamics panel to view the 3D visualization. To go back, we can simply click 
"3D" again.
<img src="../images/3d_1.png" class="center"/>

After selecting a track, we can go to the Percentage tab to see percentage of cells in each stage and in each cluster. 
<img src="../images/perc_1.png" class="center"/>

In the gene panel, we can select two clusters to compare their gene expression. Click "compare"
after selecting two clusters and the results will be shown in a few seconds.
<img src="../images/gene_3.png" class="center"/>
<img src="../images/gene_2.png" class="center"/>

<img src="../images/genetab_2.png" class="center"/>
<img src="../images/genetab_1.png" class="center"/>
