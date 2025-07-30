---
title: Cross-Section Optimization 
numbering:
  enumerator: 3.%s
---

## Optimized Cross-Section Preparation with Cryogenic Laser Ablation and Plasma Focused Ion Beam

(laser_param)=
###	Influence of Laser Parameters

Laser wavelength and polarization can influence the cross-section surface, therefore these parameters were investigated to develop an optimized cross-section workflow. In some ways, selecting the UPL wavelength and/or polarization is similar to selecting the ion species in a FIB/PFIB; one set of parameters may be more beneficial for a specific material or application. For each sample, the goal of the tuning process is to mitigate LIPSS or roughness on a UPL-ablated surface, which can appear on most classes of materials but tend to be most obvious on semiconductors and metals. LIPSS tend to appear as ripple-like features that are classified based on the pattern periodicity ($\Lambda$) of the structures: low-spatial frequency LIPSS (LSFL, $\Lambda$ ≈ laser wavelength), which usually occur perpendicular to the incident laser polarization, and high-spatial frequency LIPSS (HSFL, $\Lambda$ < laser wavelength), which can be aligned perpendicular or parallel to the incident laser. In cases where some features of interest are smaller than the spatial periodicity of LIPSS, those features could be masked; however, since LIPSS are only apparent on the surface of some materials, it can be useful for identifying LIPSS-vulnerable materials (e.g metals, semiconductors) embedded within LIPSS-invulnerable materials (e.g. nonmetals).

To showcase the importance of wavelength tuning, we contrasted identically prepared coin cell samples polished using 515 nm UPL and 1030 nm UPL, respectively. @LIPSS_515vs1030 (a) shows the ROI of the coin cell intermediate-polished using 515 nm UPL, where LSFL (average $\Lambda$ ≈ 400 nm) are primarily observed on the stainless-steel casing, Cu current collectors, and Li metal of the coin cells; aperiodic LIPSS are primarily observed on the polymer separator materials and SEI/electrolyte. @LIPSS_515vs1030 (b) shows the same region intermediate-polished with 1030 nm, where the LIPSS are more prominent on the Li metal and Cu, with a spatial periodicity of ~ 1 $\mu$m. Because the SEI/Li interface is significantly clearer with the 515 nm intermediate polish, we also used the 515 nm wavelength for the final PFIB polish, to obtain a cut face that appears smoother and allows smaller features to be resolved. Having said that, while the larger 1030 nm LIPSS are a drawback, the 1030 nm wavelength accesses higher average power and pulse energy, conveniently reducing total milling time, especially for hard-to-mill materials, including the coin cell’s stainless-steel casing. The final PFIB polish (at glancing angles) removes LIPSS remaining after the intermediate polish, further resolving small features13 and will be discussed later. To optimize characterization outcomes, we used the 1030 nm wavelength for the coarse mill (reducing milling time) and rapidly switched to the second-harmonic 515 nm wavelength for the intermediate polish (reducing beam current and voltage to minimize damage and reduce LIPSS periodicity).

:::{figure} ./figures/LIPSS_515vs1030.png
:name: LIPSS_515vs1030
Wavelength-dependent LIPSS variation on coin cell ROI. Cryo-SEM BSE images of an uncycled (pristine) coin cell battery ablated with a) 515 nm and b) 1030 nm.
:::

Because different materials will have different reflectivity for a given polarization, tuning the polarization varies both the LIPSS orientation and the cut face angle. Multiple beam paths and waveplates (integrated into laser control software) allow for the laser polarization to be instantaneous changed, which is important because LSFL (and sometimes HSFL) are typically perpendicular to the laser polarization, where the orientation of LIPSS can be rotated according to feature orientation or direction where features are least obscured by LIPSS. To clarify that importance, we studied the effect of polarization on wavelength-dependent LIPSS in identically prepared coin cells. @Pol-comparison-labeled (a) contains a region polished with p-polarized light (515 nm): the Li metal has polarization-perpendicular LSFL ripples, the LiH deposits have polarization-perpendicular HSFL ripples, and the SEI/electrolyte have slight textural variation but no observable LIPSS. @Pol-comparison-labeled (b) shows a similar region from the same coin cell polished with s-polarized light (515 nm): the Li metal has generally vertical surface structures, but no ripples; the LiH deposit has HSFL with vertical ripples; and the SEI/electrolyte has no observable LIPSS. @Pol-comparison-labeled (c) and (d) are both taken from the same coin cell (identically prepared to with the coin cell from @Pol-comparison-labeled (a) and (b)) and show a region with Li metal, SEI/electrolyte, and polymer separator. @Pol-comparison-labeled (c) was polished with p-polarized light (1030 nm) and shows LSFL only on the Li metal. @Pol-comparison-labeled (d) was polished with circularly polarized light (1030 nm) and shows LSFL as diagonal ripples only on the Li metal, but also shows slight variations in texture to the SEI/electrolyte and polymer separator.

:::{figure} ./figures/Pol-comparison-labeled.png
:name: Pol-comparison-labeled
Effect of polarization on wavelength-dependent LIPSS in coin cell ROI observed via Cryo-SEM BSE. A coin cell region with Li metal, SEI/electrolyte, and LiH deposits polished with a) p-polarization (515nm) and b) s-polarization (515 nm). A coin cell region with Li metal, SEI/electrolyte, and polymer separator polished with c) p-polarization (1030 nm) and d) circular polarization (1030 nm).
:::

While LIPSS are most often disadvantageous for the resolution of fine details, the ability to more cleanly differentiate different materials (e.g. Li metal from LiH deposits; Li metal embedded in SEI) based on LIPSS presence and periodicity can be useful. For example, @Li-deposits shows a sample polished at a 515 nm wavelength; within the SEI layer, it is easy to differentiate the Li deposits (highlighted in blue) from voids and other textures embedded the SEI, which is extremely beneficial for segmentation purposes.  

:::{figure} ./figures/Li-deposits-test.png
:name: Li-deposits
Cryo-SEM BSE images of a coin cell battery with Li metal deposits in SEI/electrolyte. The region highlighted in red on the right image is shown on the left. Li metal deposits are highlighted with blue on the right.
:::

(laser_workflow)=
### Optimized Laser Cross-Section Workflow 

A standard workflow was developed for preparing and imaging cross-sections on the coin cells to perform investigations of coin cells (i.e. with different components, cycling rates) to reveal microstructural, morphological, and composition information. After coin cells were loaded, a UPL bulk mill was used to remove the material of the targeted volume. To improve throughput, laser pattering was done in coarse mode with the longer wavelength at higher repetition rate, pulse energy, and larger pitch. This step resulted in significant redeposition of material onto the cross-section face, so an intermediate coarse polishing step was used to remove redeposition and clean the cross-section, using a smaller pattern pitch and reduced repetition rate. The UPL objective lens has a protective glass coverslip to prevent the lens from being coated by ablation debris, which is typically exchanged when changing specimen. In this case, due to the large volume of material removed and types of materials being removed, the protective coverslip would become coated after the bulk mill and coarse polish, significantly reducing the transmission of the 515 nm wavelength used for the final UPL step. The system chamber was vented and the coverslip was quickly exchanged. The sample remained at cryogenic temperatures, however a thin layer of frost could form while the cell was briefly exposed to air. 

After replacing the protective coverslip on the UPL objective lens, the final laser step sought to optimize the cross-section quality and reveal smaller scale features using 515 nm in fine patterning mode. Lower repetition rates and pulse energy were favorable for most of the components in the stack (i.e., the polymer separator materials) to reduce the likelihood of damage and heat generation from parameters that result in higher average power that is outside of the athermal ablation regime. A summary of UPL parameters used for each step is shown in the table below. Pattern times could vary depending on thickness of the cell, requiring additional passes for a thicker cell. 

```{table} Cryo UPL Table
:name: cryo-upl-table
:width: auto
:align: center

| Process        | Wavelength (nm) | Repetition Rate (kHz) | Pulse Energy (µJ) | Pattern Mode          | Pattern Dimension (µm) | Pattern Pitch (µm) | Pattern Time (min) |
|----------------|------------------|------------------------|--------------------|------------------------|-------------------------|---------------------|---------------------|
| Bulk Removal   | 1030             | 20.0                   | 40                 | Coarse (1 ms/pixel)    | 1200 x 900              | 10 x 10             | 03:36:00            |
| Coarse Polish  | 1030             | 7.5                    | 40                 | Coarse (1 ms/pixel)    | 1200 x 500              | 5 x 5               | 04:28:00            |
| Fine Polish    | 515              | 1.0                    | 10                 | Fine, 5 pulses/pixel   | 600 x 20                | 2 x 2               | 01:35:00            |
```


To optimize cut quality and reduce polishing time spent on sample areas outside of the ROI, the focus of the UPL was adjusted to the sample sub-surface; however, rather than focusing at the surface on the stainless-steel casing, we moved the objective lens in towards the sample, focusing just above the top of the battery stack layers or ROI, which significantly reduces polishing time, because it is unnecessary to polish the entire 250 $\mu$m stainless-steel casing as shown in @pattern_regions. By reducing the area that needs to be fine polished, it is possible to mill multiphase materials using a reduced ablation threshold, repetition rates, pulse energy, and pitch, without increasing the polishing time. Additionally, in some cases, the quality of the cut face can be improved by changing the angle of incidence of the laser using the stage tilt (similar to performing an under or over-cut in a traditional Ga-ion FIB). To reduce redeposition on the ROI, it is possible to use variable tilts: coarse cut (stage tilt -5&deg;, total tilt -31&deg;), coarse polish (stage -6&deg;, total -32&deg;), and final fine polish (stage -8&deg;, total -34&deg;). We note that while these are the stages and conditions applied to coin cell batteries for our previous efforts, the laser ablation parameters could easily be tuned for other purposes; for example, cut-face quality could be sacrificed to further reduce patterning time or pitch parameters could be adjusted to improve characterization quality. 

:::{figure} ./figures/pattern_regions.png
:name: pattern_regions
Cryo-SEM SE images of a coin cell battery at each UPL patterning step, where blue highlighted regions show the UPL patterned region.
:::

 (PFIB_polish)=
 ### 	Plasma Focused Ion Beam Polishing 
 
Following UPL ablation (coarse and intermediate), specific interfaces in the ROI be polished using the Xe{sup}`+` PFIB. PFIB polishing can quickly remove the LIPSS, and provide a finer surface polish to reveal smaller length scale features that are not observable from UPL prepared cross-sections. PFIB milling was done in selected regions of interest within the laser prepared cross-section, where PFIB beam conditions varied based on the morphology of the battery stack (total thickness, specific regions of interest, size of area requiring PFIB milling…), but typically operating at 30 kV and 15 – 1000 nA. However, it was necessary to physically rotate the coin cell holder 180&deg: so that the coin cell was facing the PFIB. Because the prototype system did not have a 360&deg; rotation-capable cryo-stage, it was necessary to vent the system chamber and manually rotate the sample, which is less than ideal as it exposes the sample to humid air and risks the formation of ice on the sample. Fortunately, a sufficiently rapid execution of this technique allowed the sample to be rotated and start chamber pumping in a matter of seconds. Thus, while a layer of ice did form over the cross-section during rotation, the electrolyte remained frozen and the crucial interfaces were preserved. Conveniently, it is also very easy to remove the ice layer via 30 kV PFIB, without impeding subsequent PFIB polishing in any discernable way. Although this step will be unnecessary in a 360&deg; rotation-capable cryo-stage, it may still be useful as a method for finding regions to target for cryo-liftout and TEM preparation. 

@PFIB_polish_fig (a) and (b) show a laser polished area and ROI, which was then PFIB-polished, shown in @PFIB_polish_fig (c) and (d). Note that the region in @PFIB_polish_fig (b) is a higher magnification image from the region in the red box marked in @PFIB_polish_fig (a). This cross-section was obtained in coin cell where failure occurred in the polymer separator, similar to that discussed in previous work [@10.1149/1945-7111/acf162]. Due to this failure and Li metal morphology observed in the laser cut region, this area was polished with PFIB, which is shown in @PFIB_polish_fig (c)and (d). @PFIB_polish_fig (d) contains a higher magnification image of the region marked with a red box in @PFIB_polish_fig (c). All LIPSS were removed from the surface after PFIB polishing, which revealed small Li metal domains that were not evident in the laser cut area. In addition, features and Li domains in the SEI/electrolyte which were not observed in the laser cut area are prominent in the PFIB polished region, which is particularly evident in @PFIB_polish_fig (d). 

:::{figure} ./figures/PFIB_polish.jpg
:name: PFIB_polish_fig
Cryo-SEM BSE images of a PFIB-polished coin cell battery with Li metal deposits in SEI/electrolyte. a) UPL prepared cross-section and b) higher magnification image of region marked with a red box in a). c) Image after PFIB polish on UPL prepared cross-section from a) and b), where d) shows a higher magnification image of region marked with a red box in c).
:::




