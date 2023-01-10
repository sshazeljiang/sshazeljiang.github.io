---
layout: page
menubar: docs_menu
title: Analysis - Graph Tab
show_sidebar: false
toc: true
---
analysis placeholder

We are at the graph tab upon initialization. On the left, there is a 2D visualization of the tracks. 
On the right, there is a scatter plot with different coloring options. The default coloring type of the scatter
plot is cluster. You can use the dropdown menu to select different coloring options such as cell types and genes.
<img src="../images/cluster_2.png" class="center"/>

We can hover over a
data point in the 2D visualization to see which track that cluster belongs to.
Upon clicking a cluster, a table containing the gene expression
of top genes in that cluster will be shown.

We can change the display mode to iDREM. Upon clicking a cluster
we will be directed to a new page that contains the iDREM infomation
of that cluster.


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