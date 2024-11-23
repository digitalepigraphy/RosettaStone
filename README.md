# Creating the Depth Map of the Rosetta Stone

This repository contains the raw and processed data from a collaborative project that led to the creation of the depth map and the normal map of the Rosetta Stone.

## ✍ Cite as

If you use data from this repository in your work please cite as:

Amin, M., Barmpoutis, A., Berti, M., Bozia, E., Hensel, J. and Naether, F., 2018. Depth map of the Rosetta Stone. https://dx.doi.org/10.17613/t1e2-0w02

## License

Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License (CC BY-NC-SA 4.0) https://github.com/digitalepigraphy/RosettaStone/blob/main/LICENSE.md

## Contents

### Images

1. Raw photographs from 8 different sections of the Rosetta Stone.

   - Part 1 (Upper Left): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part1
   - Part 2 (Upper Right): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part2
   - Part 3 (Middle-Upper Left): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part3
   - Part 4 (Middle-Upper Right): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part4
   - Part 5 (Middle-Lower Left): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part5
   - Part 6 (Middle-Lower Right): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part6
   - Part 7 (Lower Left): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part7
   - Part 8 (Lower Right): https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part8
   - Additional photos: https://github.com/digitalepigraphy/RosettaStone/tree/main/images/part0

2. Computed Images

   - Photo of the Rosetta Stone: https://github.com/digitalepigraphy/RosettaStone/blob/main/results/Photo_of_Rosetta_Stone.jpeg
   - Depth map of the Rosetta Stone: https://github.com/digitalepigraphy/RosettaStone/blob/main/results/Depthmap_of_Rosetta_Stone_clean.jpg
   - Normal map of the Rosetta Stone: https://github.com/digitalepigraphy/RosettaStone/blob/main/results/Normalmap_of_Rosetta_Stone.jpg

### 3D Model

1. Raw 3D scan: https://github.com/digitalepigraphy/RosettaStone/tree/main/3d_model/Raw3DModel
2. Cleaned 3D model: https://github.com/digitalepigraphy/RosettaStone/tree/main/3d_model/Cleaned3DModel
3. Composite 3D model with normal map: https://github.com/digitalepigraphy/RosettaStone/tree/main/3d_model/Rosetta3DModel
4. Screenshot of the 3D model: https://github.com/digitalepigraphy/RosettaStone/blob/main/results/3DRendering_of_Rosetta_Stone.jpg

## Scanning Method

With the permission of the British Museum, an interdisciplinary team from the University of Florida and the University of Leipzig scanned the Rosetta Stone in June 2018 to generate a high-resolution 2D and 3D map of its inscribed surface. In our setup, we used a single DSLR camera (Nikon D3400), which was fixed on a tripod in front of the stone, and calibrated as follows: exposure time = 5 sec., ISO speed = ISO-100, F-stop = f/25, focal length = 135mm, and max aperture = 4.5. To reconstruct the tridimensional inscribed surface using the shape-from-shading method, we controlled the lighting of the stone using a handheld light wand (Ice Light) that served as a 15-inch long light source of 1600 lumen at 5600k color temperature.

We divided the artifact into 8 regions (4 rows and 2 columns), which were photographed individually at 6000 x 4000 pixel resolution. Each region was photographed in 4 different lighting directions (light from the left, top, right, and bottom) by placing the light wand on the corresponding side of the region of interest. This quadri-directional lighting configuration allowed us to capture information related to the local orientation at each point of the surface through the differences in the light reflection observed in the corresponding four photographs. The entire scanning session, including opening the glass case of the artifact, setting up the equipment, digitizing the artifact, and putting everything in its original configuration before the opening of the museum took us 120 min.

## Image Processing

During this time several photographs were taken such as those included in this repository that captured 8 regions of the stone in 4 different lighting conditions. These photos were then processed to compose high-resolution 2D and 3D representations of the surface with 0.08141mm sampling frequency, which is equivalent to 312 DPI resolution (approximated as 9300px width of the picture / 29.8 inch width of rosetta stone). This corresponds to 1 pixel for 81.41 micrometers (0.08141 mm), 240 pixels height for each hieroglyphic line, 120 pixels height for each demotic line, and 90 pixels height for each Greek line.

The tridimensional details of the inscribed surface were reconstructed in the form of a normal map and a depth map, which were computed by processing the four corresponding images of the same region of interest illuminated with four different lighting orientations using the method by A. Barmpoutis, E. Bozia, and R. Wagman published in the Journal of Machine Vision and Applications 21(6) in 2010. 

Link to the paper: https://abarmpou.github.io/angelos/page/a-novel-framework-for-3d-reconstruction-and-analysis-of-ancient-inscriptions/index.html

Link to the software: https://www.digitalepigraphy.org/db/app/sfs

The normal map and the depth map contain detailed three-dimensional information on the inscribed surface so that it can be visualized in 3D. The 3D reconstructed surface can be rendered as an interactive 3D model that can be manipulated by the user (move, scale, rotate) and inspected under different virtual lighting orientations and shading methods.

## 3D Model

Finally, in addition to the 3D reconstruction of the inscribed surface, we used a hand-held laser scanner (Structure Sensor by Occipital) mounted on a tablet computer (iPad Air by Apple) to create a 3D model of the entire stone. Although the 3D model generated by this scanner can depict the overall shape of the entire artifact, it does not have enough resolution to capture the fine details of the inscribed surface. Therefore, the 3D reconstructed surface using shape-from-shading is complementary to the laser-scanned 3D model, as both of these forms can co-exist to depict different structural details of the artifact.

The result of this process is a high-resolution 3D representation of the Rosetta Stone that is available online as an interactive web app and can be accessed through the project’s website.

Link to the 3D visualization: https://research.dwi.ufl.edu/op.n/file/2fzrs3i2cvas964f/embed

## Publications

Data from this project have been used in the following publications:

Amin, M., Barmpoutis, A., Berti, M., Bozia, E., Hensel, J. and Naether, F., 2018. Depth map of the Rosetta Stone. http://dx.doi.org/10.17613/t1e2-0w02

Birk, R., 2021. "Der Rand des Rosettasteins. Eine Neulesung von Z. 1 des hieroglyphischen Texts", Chronique d'Egypte 96(191), pp.10-22. https://doi.org/10.1484/J.CDE.5.128161

Regulski, I. 2022. Hieroglyphs: Unlocking Ancient Egypt. pp. 236.

Amin, M., Barmpoutis, A., Berti, M., Bozia, E., Hensel, J. and Naether, F., 2023. The Digital Rosetta Stone Project. Chapter 3 In Ancient Egypt, New Technology: The Present and Future of Computer Visualization, Virtual Reality and other Digital Humanities in Egyptology, R. Lucarelli, J. Roberson, and S. Vinson (ed.), Harvard Egyptological Studies, vol. 17, pp. 58-84. https://doi.org/10.1163/9789004501294

Barmpoutis, A. and Bozia, E., 2023. Reinscribing the 3rd dimension in epigraphic studies and transcending disciplinary boundaries. In Numérique et lecture de textes épigraphiques altérés, H. Gonzalez Bordas and F. Comte (eds.). Pessac, Ausonius éditions, collection PrimaLun@ 27, pp. 79-94. https://ressources.una-editions.fr/s/WRjmQn8Sd2Ddp8k

Bozia, E., 2023. “Please, Touch the Exhibits”: 3D Archaeology for Experiential Spatialisation. In Capturing the Senses: Digital Methods for Sensory Archaeologies (pp. 127-147). Cham: Springer International Publishing.

Panov, M. and Lanciers, E., 2023. The Memphite Sacerdotal Decree of 161 BCE (Plates I–V). Journal of Egyptian History, 16(1), pp.30-82.

Manzetti, M.C., 2023. Combining 3D Visibility Analysis and Virtual Acoustics Analysis for the Architectural Study of Ancient Theatres. In Capturing the Senses: Digital Methods for Sensory Archaeologies (pp. 105-125). Cham: Springer International Publishing.

Birk, R. with contributions by Jonas Treptow, Simon D. Schweitzer, Altägyptisches Wörterbuch, Daniel A. Werning, 2024. "Rosettana (Égyptien de Tradition)" (Text ID FNXUNEJ2OBGDPM6HCHZJC2672Q), Thesaurus Linguae Aegyptiae, Corpus issue 19, Web app version 2.2.0, 11/5/2024, ed. by Tonio Sebastian Richter & Daniel A. Werning on behalf of the Berlin-Brandenburgische Akademie der Wissenschaften and Hans-Werner Fischer-Elfert & Peter Dils on behalf of the Sächsische Akademie der Wissenschaften zu Leipzig (accessed: 11/23/2024). https://thesaurus-linguae-aegyptiae.de/text/FNXUNEJ2OBGDPM6HCHZJC2672Q

## Additional Resources

All Good Things come in Threes: The Rosetta Stone and the Decipherment of Ancient Egyptian. https://ausstellungen.deutsche-digitale-bibliothek.de/rosetta-stone/




