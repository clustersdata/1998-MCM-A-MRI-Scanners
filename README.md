# 1998-MCM-A-MRI-Scanners


Introduction

Industrial and medical diagnostic machines known as Magnetic Resonance Imagers (MRI) scan a three-dimensional object such as a brain, and deliver their results in the form of a three-dimensional array of pixels. Each pixel consists of one number indicating a color or a shade of gray that encodes a measure of water concentration in a small region of the scanned object at the location of the pixel. For instance, 0 can picture high water concentration in black (ventricles, blood vessels), 128 can picture a low water density in white (lipid-right white matter consisting of myelinated axons). Such MRI scanners also include facilities to pictures on a screen any horizontal or vertical slide through the three-dimensional array (slices are parallel to any of the three Cartesian coordinate axes).

Algorithms for picturing slices through oblique planes, however, are proprietary. Current algorithms are limited in terms of the angles and parameter options available; are implemented only on heavily used dedicated workstations; lack input capabilities for marking points in the picture before slicing; and tend to blur and “feather out” sharp boundaries between the original pixels.

A more faithful, flexible algorithm implemented on a personal computer would be useful

    for planning minimally invasive treatments,
    for calibrating the MRI machines,
    for investigating structures oriented obliquely in space, such as post-mortem tissue sections in animal research,
    for enabling cross-sections at any angle through a brain atlas consisting of black-and-white line drawings.

To design such an algorithm, one can access the values and locations of the pixels, but not the initial data gathered by the scanner.

Problem

Design and test an algorithm that produces sections of three-dimensional arrays by planes in any orientation in space, preserving the original gray-scale values as closely as possible.

Data Sets

The typical data set consists of a three-dimensional array A of numbers A(i,j,k) which indicates the density A(i,j,k) of the object at the location (x,y,z)_{ijk}. Typically, A(i,j,k) can range from 0 through 255. In most applications, the data set is quite large. Teams should design data sets to test and demonstrate their algorithms. The data sets should reflect conditions likely to be of diagnostic interest. Teams should also characterize data sets that limit the effectiveness of their algorithms.

Summary

The algorithm must produce a picture of the slice of the three-dimensional array by a plane in space. The plane can have any orientation and any location in space. (The plane can miss some or all data points). The result of the algorithm should be a model of the density of the scanned object over the selected plane.
