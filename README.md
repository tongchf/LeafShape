# LeafShape: An R package for extracting the shap indexes of oval tree leaves

# Introduction
`LeafShape` is an R package for extracting the shap indexes of oval tree leavies, including leaf length, width, area, and radius from center to edge. The width values contain the widths at the one-third part, at the half part and at the two-thirds part as well as the largest one. The radius is taken at every degree from -pi to pi. `LeafShape` can handle a large number of leavies at the same time. Each leaf should be scanned to generate a bmp file with 24 bit RGB and a fixed resolution. All the bmp file should be saved in a same directory.
# Usage
'LeafShape' consists of three R programs, i.e., `leafshape.r`, `singleleaf.r`, and `leafFunctions.r`. 
