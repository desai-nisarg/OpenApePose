<h1 align="left">OpenApePose: a database of annotated ape photographs for pose estimation
</h1> 

<p align="center">
  <a href="#introduction">Introduction</a> |
  <a href="#Overview">Overview</a> |
  <a href="#Download">Download</a> |
  <a href="#Annotation&#32;format">Annotation format</a> |
  <a href="#License">License</a> 
</p>

## Introduction

<p align="left">This repository contians the <a href='https://www.biorxiv.org/'>OpenApePose</a> dataset. OpenApePose contains 71,868 photographs of of six ape species in naturalistic contexts. All images are annotated with 16 body landmarks described below. </p>

## Overview

### Number of images per species

<p>
<table div align=center>
  
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
</p>

### Keypoint definition
<p align="center">
<img src="overview_images/keypoints.jpg" width="500">
</p>



### Overview of annotations
<p align="center">
<img src="overview_images/collage.png" width="1300">
</p>



## Download

The dataset can be downloaded from
<a href='https://drive.google.com/drive/folders/1bEXBHoPgmUPOWB898tXTHJznzGpAucOG?usp=share_link'>[Google Drive]</a> <a href='https://umn.box.com/s/1kgz8had6tvvzb5c0xhdfdky0xcjoq7m'>[Box]</a>

The downloaded dataset would look as follows:

```text
|── OpenApePose
    │-- annotations
    │   │-- oap_all.json
    │   |-- oap_test.json
    │   |-- oap_train.json
    │   |-- oap_val.json
    │-- data
    │   │-- 00001_oap.JPG
    │   │-- 00002_oap.jpg
    │   │-- ...

```

## Annotation format

```text
{
"data": [
{ 
"file":   str, 
"species":   str, 
"bbox":   [x, y, width, height], 
"landmarks":   [x1,y1, ...,x16,y16],
"visibility":   [v1,v2,...,v16]
},
{ 
"file":   str, 
"species":   str, 
"bbox":   [x, y, width, height], 
"landmarks":   [x1,y1, ...,x16,y16],
"visibility":   [v1,v2,...,v16]
},
....
]
}
```


## License

The dataset follows CC-BY-4.0 license.

## Cite as
Desai, N., Bala, P., Richardson, R., Raper, J., Zimmermann, J., & Hayden, B. (2022). OpenApePose: a database of annotated 
ape photographs for pose estimation.
