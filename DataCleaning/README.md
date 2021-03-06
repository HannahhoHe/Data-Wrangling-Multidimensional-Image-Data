# What is the script for?
- There are 50-60 files of images from different specimens, all with DBSCAN cluster ID appended (after DBSCAN clustering). The script is to uniform the column names and the phenotype names, originally labelled with various forms.
- In addition, there are two steps of assigning cluster ID to the cells. In the first step, we performed the DBSCAN clustering based on a subset of cell types (of our interest), with which the results are shown in the column called "DBSCAN Cluster". In the second step, we followed the cells at the resultant cluster periphery, and we further assigned the cluster ID to the cells that do not participate in the first clustering process. Results from the new cluster assignment are shown in the column "Belong to DBSCAN0". In some cases, cells can belong to more than one unique cluster due to the cluster overlap. As such, an additional column(s) "Belong to DBSCAN1", "Belong to DBSCAN2"...., will be generated. 
- For every file, after standardizing the names, and with some columns extracted, a new file is generated and renamed by its "Path" content. 
- At the end of the script, all the new files are called and merged to one giant file. 


