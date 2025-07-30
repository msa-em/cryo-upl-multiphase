---
title: Characterization of 3D Volumes
numbering:
  enumerator: 4.%s
---

(characterzation)=
# Characterization Approaches for Large 3D Volumes

To better understand the mechanisms that drive the behavior of complex multiphase materials systems (including coin cells whose heterogeneity is increased over the course of battery cycling {cite:p}`jungjohann2021cryogenic`), it is useful to analyze both representative areas and volumes. Previously, MicroCT and NanoCT have been used to non-destructively study 3D structures within partial and complete battery stacks{cite:p}`lu20203d`. We were able to obtain high-quality cross-sections of the coin cells, with vastly improved clarity in the ROI compared to MicroCT (@UPL_SEM , @MicroCT ). @UPL_SEM (a) shows a sample after UPL ablation was performed to remove bulk material (~ 1 x 0.9 x 0.7 mm), including the steel casing), around the cell ROI which is outlined in red. We can clearly resolve interfaces between the casing, copper current collectors, electrolyte, solid electrolyte interphase (SEI), polymer separator, and lithium metal. @UPL_SEM (b) shows higher magnification for the ROI, revealing the cell morphology. For clarity, we have applied false color to the image, clearly distinguishing lithium metal deposits embedded in the electrolyte + SEI layer. @MIcroCT (a) shows MicroCT data collected on a Zeiss 560 Nano Focus, which shows the full coin cell assembly (spacers, casing, etc.); @MicroCT (d) shows a magnification of the ROI (current collectors, Li, electrolyte/SEI, separator) with extremely low-resolution. To emphasize the comparatively high quality of this image, we would like to highlight that all components in the ROI are distinguishable in the UPL-prepared cross-section SEM image (@UPL_SEM (b)) whereas no details are distinguishable in the equivalent ROI by MicroCT (Figure 2d). Based on EDS , BSE image contrast, and LIPSS that differ between SEI vs. Li (discussed in @laser_param ) deposits of Li metal could be identified in the top electrolyte + SEI layer. However, as shown in @UPL_SEM, MicroCT of a coin cell can show the complete stack, but cannot resolve or differentiate key components in the ROI (e.g. electrolyte/SEI, separator, and Li metal) due to the low X-ray transparency of the stainless-steel casing, which increases the number of imaging artifacts. A recently demonstrated transparency window offers a promising avenue for future enhancements in MicroCT resolution but, at present, this technique is still poorly suited for resolving stack components in an assembled coin cell because the window can compromise the electrochemical properties {cite:p}`tan2018evolution`.

:::::{tab-set}

::::{tab-item} Cryo UPL-prepared cross section
:sync: tabmovie1

:::{figure} ./figures/cryoUPL_Large FOV.png
:name: UPL_SEM

*Comparison of UPL-prepared SEM and MicroCT characterizations on the same representative ROI in identically prepared half coin cells with concentrated basalt electrolyte cycled to 100.5 cycles at low rate.* a) Overview of a cryo-SEM secondary electron cross-section image collected at 5 kV, 0.69 nA of a ~ 1 x 0.9 x 0.7 mm region in a coin cell battery removed with UPL ablation, where the ROI is marked with a red box. b) Higher magnification cryo-SEM backscatter electron (BSE) image of the ROI collected at 2 kV, 0.69 nA. 
:::

::::

::::{tab-item} MicroCT
:sync: tabmovie2

:::{figure} ./figures/microCT.png
:name: MicroCT
*Comparison of UPL-prepared SEM and MicroCT characterizations on the same representative ROI in identically prepared half coin cells with concentrated basalt electrolyte cycled to 100.5 cycles at low rate.* a) MicroCT scan of full coin cell assembly. b) Virtual slice from the ROI region marked with red box in a).
:::

::::

:::::



Fortunately, the Laser PFIB can be used to collect high-quality automated ‘slice-and-view’ data, alternately using UPL ablation and SEM imaging to capture slices of data that can then be reconstructed to obtain a 3D dataset. Depending on the quality of 3D imaging required, slice thickness can be adjusted by moving the beam or stage positions; using the most recently developed Helios Laser PFIB, more advanced automated (e.g. EDS, ESBD) workflows can also be incorporated. For our initial 3D demonstration, we used the prototype Helios Laser PFIB to create 2.5 $\mu$m slices and capture back scattered electron (BSE) images of each slice, as shown in @SEM_2D_slicer. To eliminate the redeposition at the edges of the sliced field of view, the images were cropped from 500 $\mu$m to 316 $\mu$m; however, as an alternative to cropping, it should be possible to prepare a post to remove material from both sides of the ROI. Our images were aligned with reference to the Cu current collectors and polymer separator. The slices (total volume 316 x 281 x 152 $\mu$m) were then reconstructed with Avizo software to reveal a segmented reconstruction of the Cu, Li metal, and polymer separator (@volume_render_3d ). The results offer unique insight into the sample’s morphology, while retaining nanoscale resolution for each of component of the multiphase system. Qualitative observation of the uniformity of the Cu current collectors showed variation in both roughness and thickness. Further study of the Li morphology on either side of the separator showed that pits on the bottom of the Li layer correspond to protruding Li grains on the top of the Li layer, which are not obvious in single frames a cross-sectional area in @2d_volume_slice . 

:::{figure} #app:3d_volume_render
:name: volume_render_3d
:placeholder: ./figures/volume_renderer_placeholder.png
3D reconstruction of automated laser slice-and-view collection in a coin cell showing segmented Cu (yellow) and Li metal (blue). The polymer separator and liquid electrolyte have been excluded to show disconnected Li metal.
:::

:::::{tab-set}

::::{tab-item} 2D Volume Slicer of Segmented Li Metal and Cu
:sync: tabmovie2

:::{figure} #app:2d_volume_slice
:name: 2d_volume_slice
:placeholder: ./figures/2D_seg_placeholder.png.png
2D slice-and-view of automated laser coin cell crosssection showing segmented Cu (yellow) and Li metal (blue). The polymer seporator and liquid electrolyte have been excluded to show disconnected Li metal.
:::

::::

::::{tab-item} 2D Volume Slicer of SEM images
:sync: tabmovie2

:::{figure} #app:SEM_2D_slicer
:name: SEM_2D_slicer
:placeholder: ./figures/2D_SEM_placeholder.png
2D slice-and-view of automated laser coin cell crosssection Cryo-SEM images.
:::

::::

:::::
