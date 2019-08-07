# LeafShape: An R package for extracting the shape indexes of oval tree leaves

# Introduction
`LeafShape` is an R package for extracting the shape indexes of oval tree leavies, including leaf length, width, area, and radius from center to edge. The width values contain the widths at the one-third part, at the half part and at the two-thirds part as well as the largest one. The radius is taken at every degree from -pi to pi. `LeafShape` can handle a large number of leavies at the same time. Each leaf should be scanned to generate a bmp file with 24 bit RGB and a fixed resolution. All the bmp file should be saved in a same directory.
# Usage
`LeafShape` consists of three R scripts, i.e., `leafshape.r`, `singleleaf.r`, and `leafFunctions.r`. Two steps are needed to perform the computations for multiple leaves with this software. The first step is to run the command:
```
  Rscript leafshape.r -p 1 -b bmppath -d outpath
```
where the paramter `p` taking the value of 1 stands for the first step,  `b` for the path of bmp files, and `d` for the ouput path. After finishing the run, two folders, i.e., csv and pdf, will be created in the output folder. In the folder of csv, there are four files for each leaf, which contain the data of leaf length, width, and area as well as 360 polar radii. In the pdf folder, each leaf has a pdf file that records the image processes. With this pdf file, users can check if the data of the leaf is successfully extracted. If a few leaves fail in the extracting process, please delete the corresponding files in the csv folder or reprocess the leaves.  
  
  Next, the second step can be run with the command:
  ```
  Rscript leafshape.r -p 2 -d outpath
  ```
  where the paramter `p` taking the value of 2 refers to the second step and `d` for the ouput path. This step will generate two files in the ouput folder, namely `AllSamplesLWA.csv` and `AllSamplesPD360.csv`. The first file contains the leaf length, width, and area for all the samples, while the second includes the 360 polar radii for each leaf.
