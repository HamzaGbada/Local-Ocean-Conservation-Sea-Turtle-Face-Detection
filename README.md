# Local Ocean Conservation Sea Turtle Face Detection

## Description
Being able to identify individual animals is a critical aspect of modern conservation. In the case of sea turtle conservation efforts, tracking where and when individuals are spotted can help reveal patterns of movement and residency, and allow more accurate estimates of population. Sea turtles can be identified using their facial scales, which are as unique as a human fingerprint.

Local Ocean Conservation (LOC) would like to use the unique fingerprint of turtle faces to integrate facial image recognition into their existing turtle applications, which would speed up many routine conservation tasks. As a first step towards such a system, we need to develop a tool that can crop a given image to show only the important facial region, reducing the chances of an accidental match down the line.

The goal of this competition is to develop an algorithm or model that can take in an image of a sea turtle and output the position of a bounding box around that all-important scale pattern. A labelled training set with bounding box annotations has been provided.

Competition was run by [Zindi](https://zindi.africa/) on their platform ([competition link](https://zindi.africa/competitions/local-ocean-conservation-sea-turtle-face-detection))

## Evaluation

The evaluation metric for this competition is Intersection-over-Union (IoU - more information on this metric in this article: [IoU](https://www.pyimagesearch.com/2016/11/07/intersection-over-union-iou-for-object-detection/))

You must specify the extent of the bounding box as shown in the sample submission file, specifying x, y, width and height as floats between 0 and 1 (fractions of the image extent). The bounding box coordinates in pixels are:

```
  x1, y1, x2, y2 = (x*image_width), (y*image_height), ((x+w)*image_width), ((y+h)*image_height)

```
