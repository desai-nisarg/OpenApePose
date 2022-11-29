<h1 align="left">OpenApePose: a database of annotated ape photographs for pose estimation
</h1> 

<p align="center">
  <a href="#introduction">Introduction</a> |
  <a href="#Overview">Overview</a> |
  <a href="#download">Download</a> |
  <a href="#license">License</a> 
</p>

## Introduction

<p align="left">This repository contians the <a href='https://www.biorxiv.org/'>OpenApePose</a> dataset. OpenApePose contains 71,868 photographs of of six ape species in naturalistic contexts. All images are annotated with 16 body landmarks described below. </p>

## Overview

### number of images per species and keypoint definition

<p>
<table div align=left>
  
<tbody>
  <tr>
    <td><b>Species</b></td>
    <td>Bonobos</td>
    <td>Chimpanzees</td>
    <td>Gibbons</td>
    <td>Gorillas</td>
    <td>Orangutans</td>
    <td>Siamangs</td>
  </tr>
  <tr>
    <td><b>Images</b></td>
    <td>11,685</td>
    <td>18,010</td>
    <td>9,274</td>
    <td>12,905</td>
    <td>12,722</td>
    <td>7,272</td>
</tbody>
</table>
<img src="overview_images/keypoints.jpg" width="500">
</p>



### Overview of annotations
<p align="center">
<img src="overview_images/collage.png" width="1300">
</p>



## Download

The dataset can be downloaded from <a href='#download'>Download</a> 

The downloaded dataset would look as follows:

```text
OpenApePose
|── data
    │-- annotations
    │   │-- oap_all.json
    │   |-- oap_train.json
    │-- data
    │   │-- 00001_oap.JPG
    │   │-- 00002_oap.jpg
    │   │-- ...

```


## License

The dataset follows CC-BY-4.0 license.
