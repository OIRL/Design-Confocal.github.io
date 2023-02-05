---
title: "Implementation of a confocal microscope using Thorlabs components"
layout: post
---

Confocal microscopes are known for optically removing the out-of-focus information (i.e., blur) in each transverse section of the sample’s volume, 
providing a more accurate three-dimensional image of thick microscopic samples than widefield microscopes. In this work, we have designed and evaluated 
a confocal microscope using off-of-shelf optical components from Thorlabs’ catalog, one of the major optical manufacturers. The design and evaluation have been 
implemented using Zemax OpticStudio, the standard optical system design software. Here, we have also reported a practical protocol for building a confocal microscope 
using sequential mode. 

### BACKGROUND OF CONFOCAL MICROSCOPY

A confocal microscope is composed of two subsystems: the illumination and detection systems. Figure 1 shows the optical configuration of a confocal system.
The monochromatic light emitting from a laser source is collimated and focused onto the three-dimensional sample by a microscope objective lens. Although the
focused beam illuminates all parts of the sample within the illumination cone, the small region surrounding the beam's focus receives the highest illumination energy. 
Assuming that the illumination wavelength is within the excitation band of the fluorescent dye, the sample’s region stained by those fluorophores are activated, 
emitting fluorescent light (e.g., light with a longer wavelength than the illumination wavelength). 
In traditional confocal microscopes, the detection system is composed of the microscope objective lens, the tube lens, a pinhole (e.g., an optical aperture),
and a photomultiplier as a detector. The fluorescent light scattered by the sample is collected by the microscope objective lens and focused on the pinhole thanks to
the tube lens. The photomultiplier is the ideal photometric detector for this imaging modality based on its speed and sensitivity. Experimentally, the photomultiplier
is placed right after the pinhole to collect the maximum amount of light. 
As previously mentioned, the feature of confocal microscopy is its optical sectioning capability (i.e., the optical removal of the out-of-focus information). 
This capability is a consequence of the fact that the object focal plane of the objective lens is conjugated with a pinhole plane. Therefore, parts of the sample outside the in-focus plane (e.g., object focal plane of the objective lens) are not conjugated with the pinhole (e.g., image plane), reducing the probability of fluorescent light detection. In other words, point-based detection using the pinhole is responsible for providing optical sectioning capability. On the other hand, parts of the sample outside the in-focus plane receive a smaller illumination density, reducing the probability of fluorescent emission and photobleaching of the samples. 

<img src="figures/Picture1.png" 
     width="400" 
     height="300"
     class="center" />
<br>
[Fig. 1. Optical configuration of a Confocal Microscope. The key feature of the point-based illumination and detection.]
