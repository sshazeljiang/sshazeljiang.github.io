---
layout: page
menubar: docs_menu
title: Tutorial - Explore Graph Tab
subtitle: Tutorials
show_sidebar: false
toc: true
---
Tutorial - Explore Graph Tab
---
<img src="../../../images/graph_tab.png" class="center"/>
The graph tab contains 2D and 3D visualization of the progression
of cell behaviour in IPF patients and a umap section.

## 2D Visualization of Clusters
On the left of graph tab, there is a 2D visualization of the progression
of cell behaviour in IPF patients. When you hover a cluster,
the tracks in which it belongs to will be highlighted. You can disable
the hover track feature by clicking the 'Hover Track' button
in the path selection panel in the sidebar.
<p align="center">
    <img src="../../../images/hover_track.png" width="50%" />
</p>

You can also use the sidebar to draw specific tracks.
Please navigate to the Path Selection panel under Dynamics Panel.
You can select the clusters you want to investigate using the dropdown menus.
Once you select a control cluster, the clusters in IPF 1, 2, 3 will be automatically filled in.
<p align="center">
    <img src="../../../images/panels_cluster.png" width="30%" />
</p>
After you finish selecting, click 'Confirm Track'.

Now you can click the 'Draw' button to highlight the selected clusters.
<p align="center">
  <img src="../../../images/draw.png" width="90%" />
</p>

You can use the 'Reset' button to clear your selection.

## 3D Visualization of Clusters
You can click the '3D' button to see the 3D visualization of how the maps of each IPF stage 
are connected. The selected track will be highlighted.
You can click again to return the 2D visualization.
<p align="center">
  <img src="../../../images/3D.png" width="90%" />
</p>

## Umaps
On the right of graph tab is the umap section.
You can use the two dropdown menus to choose which
umap you would like to display.
<p align="center">
    <img src="../../../images/umap_1.png" width="32.4%" />
    <img src="../../../images/umap_2.png" width="32.4%" />
    <img src="../../../images/umap_3.png" width="32.4%" />
</p>

## Display Mode
There are three display mode: DEG, iDREM, and Highlight on Umap.
We will explain each in details below.
<p align="center">
    <img src="../../../images/display_mode.png" width="50%" />
</p>

### DEG
The default display mode is DEG. Under DEG mode, when you click a cluster,
a table will pop out showing the gene expression of top genes in
that cluster.
<p align="center">
    <img src="../../../images/gene_expr.png" width="90%" />
</p>

### iDREM
Under this mode, when you click a cluster with a complete track,
you will be directed to a new iDREM page. If the cluster you
clicked doesn't have a complete track, a notification will
pop up.
<p align="center">
    <img src="../../../images/idrem_1.png" width="90%" />
    <img src="../../../images/idrem_2.png" width="90%" />
</p>

### Highlight on Umap
Under this mode, when you click a cluster, that cluster will be
highlighted in the umap.
<p align="center">
    <img src="../../../images/highlight_on_umap.png" width="90%" />
</p>