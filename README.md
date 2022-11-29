<h1 align="left">OpenApePose: a database of annotated ape photographs for pose estimation
</h1> 

<p align="center">
  <a href="#introduction">Introduction</a> |
  <a href="#Overview">Overview</a> |
  <a href="#Download">Download</a> |
  <a href="#Annotation-format">Annotation format</a> |
  <a href="#License">License</a> 
</p>

## Introduction

<p align="left">This repository contians the <a href='https://www.biorxiv.org/'>OpenApePose</a> dataset. OpenApePose contains 71,868 photographs of six ape species in naturalistic contexts. Because of their close relationship with humans, non-human apes (chimpanzees, bonobos, gorillas, orangutans, and gibbons, including siamangs) are of great scientific interest. The goal of understanding their complex behavior would be greatly advanced by the ability to perform video-based behavioral tracking. Tracking, however, requires high-quality annotated datasets of ape photographs. Here we present a new public dataset of 71,868 photographs, annotated with 16 body landmarks, of six ape species in naturalistic contexts. </p>

<p align="center">
<img src="overview_images/collage.png" width="1300">
</p>

## Overview

<p align="left">The dataset includes species from the ape (<i>Hominoidea</i>) superfamily. This includes the great apes (<i>Hominidae</i> family) and the lesser apes, gibbons and siamangs (<i>Hylobatidae</i> family). Among the <i>Hominidae</i>, we include four species: bonobos (<i>Pan paniscus</i>), chimpanzees (<i>Pan troglodytes</i>), gorillas (<i>Gorilla gorilla</i>), and orangutans (<i>Pongo sp.</i>). Among the gibbons we separate the siamangs (<i>Symphalangus syndactylus</i>) but include other species under the "gibbon" label. Below is the number of images from each of these species.  </p>

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

<p align="left">We include 16 landmarks in the following order: Nose, Left eye, Right eye, Head, Neck, Left shoulder, Left elbow, Left wrist, Right shoulder, Right elbow, Right wrist, Hip/Sacrum, Left knee, Left foot, Right knee, Right foot </p>
<p align="center">
<img src="overview_images/keypoints.jpg" width="500">
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
    │-- images
    │   │-- 00001_oap.JPG
    │   │-- 00002_oap.jpg
    │   │-- ...

```

## Annotation format

<p align="left">Our annotation format is inspired from other similar datasets such as <a href='https://idp.springer.com/authorize/casa?redirect_uri=https://link.springer.com/article/10.1007/s11263-022-01698-2&casa_token=kBSmHxBJToAAAAAA:mKpt4xKGExOp6471wnf2AB-bGka2o1A_rdih4VHg0yffT1sllepqI5c5R0nwtT1vt4bqiLKQdic5XnM'>OpenMonkeyPose</a>, <a href='https://cocodataset.org/#keypoints-2017'>COCO</a> etc. They are provided as separate JSON files for the full dataset, as well as train, validation, and test set splits used in the original <a href='https://www.biorxiv.org/'>OpenApePose</a> paper. The downloaded dataset should look as follows: </p>

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
<p align="left">Within each JSON file, all the annotations are included in the "data" tag. Each annotation contains the following tags: "file", "species", "bbox", "landmarks", and "visibility". "file" specifies the name of the file in the images folder. "species" specifies the species of the individual ape in the bounding box that is annotated. "bbox" specifies a bounding box in the image that contains the annotated ape. The bounding box format used is [x,y,width,height] where [x,y] specifies the x and y corridnate of the top-left of the bounding box, width specifies the width of the bounding box in pixels, and height specifies the height of the bounding box in pixels. "landmarks" specifies the x and y coordinates of the 16 landmarks in the order specified above. "visibility" specifies whether a given landmark is occluded (0) or visible (1).

## License

The dataset follows CC-BY-4.0 license.

## Cite as
Desai, N., Bala, P., Richardson, R., Raper, J., Zimmermann, J., & Hayden, B. (2022). OpenApePose: a database of annotated 
ape photographs for pose estimation.
