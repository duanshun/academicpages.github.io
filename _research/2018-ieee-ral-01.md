---
title: "Deep Geometric Learning"
collection: research
permalink: /research/2018-ieee-ral-01
image: "/images/18-ieee-ral-01-teaser.png"
imagedesc: 'Primitive fitting on a simulated test range image
(top left) with BAGSFit (middle right) vs. RANSAC (top
right). Estimated normals (middle left) and ground truth
labels (bottom left) are used to train a fully convolutional segmentation
network in BAGSFit. During testing, a boundaryaware
and thus instance-aware segmentation (bottom right)
is predicted, and sent through a geometric verification to fit
final primitives (randomly colored). Comparing with BAGSFit,
the RANSAC-based method produces more misses and
false detections of primitives (shown as transparent or wireframe),
and thus a less appealing visual result.'
excerpt: 'This project aims to obtain the parametric model of basic primitives from noisy point cloud.'
---


To identify and fit geometric primitives (e.g.,
planes, spheres, cylinders, cones) in a noisy point cloud is
a challenging yet beneficial task for fields such as robotics
and reverse engineering. As a multi-model multi-instance fitting
problem, it has been tackled with different approaches
including RANSAC, which however often fit inferior models
in practice with noisy inputs of cluttered scenes. Inspired by
the corresponding human recognition process, and benefiting
from the recent advancements in image semantic segmentation
using deep neural networks, we propose BAGSFit as a
new framework addressing this problem. Firstly, through a
fully convolutional neural network, the input point cloud is
point-wisely segmented into multiple classes divided by jointly
detected instance boundaries without any geometric fitting.
Thus, segments can serve as primitive hypotheses with a
probability estimation of associating primitive classes. Finally,
all hypotheses are sent through a geometric verification to
correct any misclassification by fitting primitives respectively.
We performed training using simulated range images and tested
it with both simulated and real-world point clouds.

<div align="center">
  <img src="/images/18-ieee-ral-01-teaser.png" width="700px" />
  <p>Primitive fitting on a simulated test range image
(top left) with BAGSFit (middle right) vs. RANSAC (top
right). Estimated normals (middle left) and ground truth
labels (bottom left) are used to train a fully convolutional segmentation
network in BAGSFit. During testing, a boundaryaware
and thus instance-aware segmentation (bottom right)
is predicted, and sent through a geometric verification to fit
final primitives (randomly colored). Comparing with BAGSFit,
the RANSAC-based method produces more misses and
false detections of primitives (shown as transparent or wireframe),
and thus a less appealing visual result.</p>
</div>

