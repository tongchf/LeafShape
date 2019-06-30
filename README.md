# Stovl: An R package for extracting the shap values of ovate tree leaves

# Introduction
`stovl` is an R package for extracting the shap values of ovate tree leavies, including leaf length, width, and radius from center to edge. The width values contain the widths at the one-third part, at the half part and at the two-thirds part as well as the largest one. The radius is taken at every degree from -pi to pi. `stovl` can handle a large number of leavies at the same time. Each leaf should be scanned to generate a bmp file with 24 bit RGB and a fixed resolution. All the bmp file should be saved in a same directory.
# Usage
'stovl' consists of three R programs, i.e., `stovl.r`, `leafsd.r`, and `stovlFunctions.r`. 
