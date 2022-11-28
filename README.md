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

<p align="center">
<img src="overview_images/Figure 2.pdf" width="700">
</p>

<table div align=left>
<thead>
  <tr>
    <th>Species</th>
    <th>Images</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Bonobos</td>
    <td>11,685</td>
  </tr>
  <tr>
    <td>Chimpanzees</td>
    <td>18,010</td>
  </tr>
  <tr>
    <td>Gibbons</td>
    <td>9,274</td>
  </tr>
  <tr>
    <td>Gorillas</td>
    <td>12,905</td>
  </tr>
  <tr>
    <td>Orangutans</td>
    <td>12,722</td>
  </tr>
  <tr>
    <td>Siamangs</td>
    <td>7,272</td>
  </tr>
</tbody>
</table>

### Annotations Overview
<p align="center">
<img src="overview_images/collage.png" width="700">
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
