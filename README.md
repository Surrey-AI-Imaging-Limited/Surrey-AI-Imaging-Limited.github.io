![Logo](https://surrey-ai-imaging-limited.github.io/pictures/logo2.png)


# Introduction

Surrey AI Imaging Limited (SAIIL) is a technology startup located in Surrey, UK that specialises in image processing and AI, particularly in the areas of planetary remote sensing and Earth observation. With extensive experience in computer vision, remote sensing, machine learning, and deep learning, the technical team at SAIIL possesses a comprehensive understanding of image processing algorithms, deep learning models, and their applications to solve complex and challenging problems in planetary and Earth remote sensing. Our expertise encompasses the following applications:

- Satellite image and video super-resolution restoration, including restoration of low-resolution (500 m - 1 km), high-resolution (20 m – 4 m), and ultra-high-resolution (30 cm – 1 m) imagery and videos, as well as from visible bands (panchromatic and RGB) and multispectral bands.
- Photogrammetry, photoclinometry, structure from motion and monocular height estimation based 3D reconstruction (i.e., digital terrain modelling, topographic mapping).
- Subpixel-scale 3D reconstruction using coupled deep learning based image super-resolution and monocular height estimation. 
- Satellite image shadow detection, deshading and reshading using deep learning.
- Satellite image matching, multi-resolution image co-registration and mosaicing.
- Optical flow and 3D scene flow based feature and scene tracking, such as cloud masking and cloud motion vector retrieval.
- Object and ground feature detection, segmentation, classification, and tracking for buildings, cars, airplanes, trees, people on the Earth, and rocks, craters, layers, and dynamic surface features on planetary surfaces.
- Imaging and geospatial data analytics including image effective resolution measurements, multi-spectral statistics, geocalibration and camera model transformations and analysis.
- GPU optimisations and onboard "smart-sattelite" solutions of remote sensing applications.

SAIIL is dedicated to providing innovative and cutting-edge solutions to address the challenges faced in the field of satellite imaging and planetary remote sensing.


# People

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/pictures/crop-jiao.jpg" alt="Kejing Zhu" width="100%">
      <p>Kejing Zhu: Director and Company Secretary</p>
      <p>Kejing Zhu brings SAIIL her leadership experience in fast growth technology start-ups of various sizes and across different industries including new media, data analysis, advertising business, remote sensing applications, education and outreach. She was previously Director of Cross Culture Communications Ltd. and has a background in accounting and marketing communications. Kejing has a M.A. degree in Interpreting from Middlesex University, London.</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/pictures/crop-dou.jpg" alt="Yu Tao" width="100%">
      <p>Dr. Yu Tao, Ph.D.: Technical Director</p>
      <p>Yu Tao has extensive experience in the remote sensing industry and plantary science with a unique mix of expertise in computer vision, machine learning and deep learning, planetary remote sensing and Earth observation systems as well as software engineering. He has a long track record of successfully leading complex software engineering projects and achieving technology breakthroughs on challenging tasks. Prior to his work with SAIIL, Yu was a senior research scientist at the University College London where he led and developed cutting-edge AI and computer vision software for plantary remote sensing and Earth observation applications. Yu has served as the lead researcher and software engineer in three European Commission 7th Framework – Space projects and as a co-investigator and project manager in two UK Space Agency Centre for Earth Observation and Instrumentation (CEOI) funded Earth observation initiatives. Yu holds a Ph.D. in Planetary 3D Imaging from the University College London and is currently serving as an Honorary Research Fellow at the same institution.</p>
    </td>
  </tr>
</table>

# Our work

**Large Area High-Resolution 3D Mapping of Mars.**

Large area, high-resolution, three-Dimensional (3D) mapping of the Martian surface is not only essential for performing key science investigations of the generation and evolution of the planet’s surface, but also critical for supporting existing and future surface robotic missions as well as human exploration. In this work, we demonstrate an end-to-end application of our in-house photogrammetric pipeline for 3D mapping of Valles Marineris, the largest system of canyons in the Solar System, using ESA Mars Express High Resolution Stereo Camera orbital images. In parallel, we demonstrate an application of our in-house deep learning-based surface modelling system to produce three large area 3D mapping products from single images taken from the ESA Mars Express High Resolution Stereo Camera (HRSC), the NASA Mars Reconnaissance Orbiter’s Context Camera (CTX), the ExoMars Trace Gas Orbiter (TGO) Colour and Stereo Surface Imaging System (CaSSIS) images, and the High Resolution Imaging Science Experiment (HiRISE) imaging data over the ExoMars 2022 Rosalind Franklin rover’s landing site at Oxia Planum on Mars. Both of the two 3D mapping products were made available through the ESA Guest Storage Facility and are being intensively exploited by the ExoMars' geological mapping team and visualisation team.

<img src="https://surrey-ai-imaging-limited.github.io/demos/OP-Mapping.png" alt="3D Mapping" width="100%">
<p>(1) An overview of the 3D mapping area at Oxia Planum (centred at 18.239°N, 24.368°W), showing the ESA Rosalind Franklin rover 1-sigma (red) and 3-sigma (green) landing ellipse areas and the ExoMars team’s geological characterisation area (blue). Shown in the background are the co-registered input datasets of MOLA DTM (colourised and hill-shaded), cropped HRSC MC-11W level 5 ORI greyscale mosaic, CTX ORI mosaic, and HiRISE image footprints (in yellow; with hatched outlines referring to those available with off-nadir stereo; the footprints are relevant to the NASA release data of 9 June 2021).</p>
<p>(2) Our 12 m CTX deep learning based DTM mosaic in comparison to the 18 m CTX photogrammetric DTMs and the 6 m CTX orthorectified images. The 1st column shows overviews of the images and DTMs, and the 2nd to the 5th columns show the zoom-in views of four different areas (locations are labelled in the overview image).</p>
<p>(3) Our 50 cm HiRISE deep learning based DTM mosaic (consisting of 44 HiRISE single-strip DTMs) in comparison with the official 1 m HiRISE PDS DTMs (photogrammetric results) and the 25 cm HiRISE images.</p>
<p>(4) Zoom-in views of two non-cherry-picking areas of the 50 cm HiRISE deep learning based DTM mosaic, the official 1 m HiRISE PDS DTMs, and the 25 cm HiRISE images.</p>

**Super-3D: subpixel-scale 3D reconstruction from Mar remote sensing imagery using deep learning based image super-resolution and monocular height estimation.**

High-resolution digital terrain models (DTMs or 3D models) play an important role in studying the formation processes involved in generating a modern-day planetary surface such as Mars. However, it has been a common understanding that DTMs derived from a particular imaging dataset can only achieve a lower, or at the best, similar effective spatial resolution compared to the input images, due to the various approximations and/or filtering processes introduced by the photogrammetric and/or photoclinometric pipelines. With recent successes in deep learning techniques, it is now become feasible to improve the effective resolution of an image using super-resolution restoration (SRR) networks, retrieving pixel-scale topography using single-image DTM estimation (SDE) networks, and subsequently, combine the two techniques to produce subpixel-scale topography from only a single-view input image. 

![Super-3D](https://surrey-ai-imaging-limited.github.io/demos/Super-3D.png)
Examples of CaSSIS Super-3D products for Oxia Planum: the landing site of the ESA ExoMars Rosalind Franklin rover. Zoom-out views (from left to right, top to bottom): An example of the 4 m CaSSIS NPB band images, 1 m CaSSIS PAN band super-resolution resolved images, intensity adjusted and blended mosaic from the 1 m CaSSIS PAN band super-resolution resolved images, 2 m CaSSIS Super-3D digital terrain model (colourised by height), 2 m CaSSIS Super-3D shaded relief image. Zoom-in views: input 4 m TGO CaSSIS image (upper-left); output 1 m CaSSIS super-resolution resolved image (upper-right); output 8 m CaSSIS 3D model using monocular height estimation (lower-left); output 2 m CaSSIS Super-3D model using coupled image super-resolution and monocular height estimation (lower-right).

<iframe width="1050" height="591" src="https://www.youtube.com/embed/yWI2DLFdk_g" title="Super-3D: subpixel-scale 3D reconstruction from Mar remote sensing imagery using deep learning" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
Subpixel-scale 3D reconstruction from Mar remote sensing imagery explained.

**Super-resolution restoration of ultra-high-resolution satellite images.**

Increasing the spatial resolution of spaceborne imagery and video using ground-based processing, or, where feasible, onboard a smart satellite, allows greater amounts of information to be extracted about the scene content. Such processing is generally referred to as super-resolution restoration (SRR). SRR techniques are applicable to images and videos without the usual increased costs and mass, associated with increased bandwidth or larger/heavier optical components, normally required for achieving higher resolution. In particular, enhancing the ultra-high spatial resolution Earth observation (EO) images, or high definition (HD) videos, is an active driver for many applications in the fields of agriculture, forestry, energy and utility maintenance and urban geospatial intelligence. The ability to further improve 30 cm/80 cm EO images and videos into 10 cm/30 cm resolution SRR images and videos will allow EO analytics to be performed in transformative ways.

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/EO-HR-SRR.png" alt="EO HR EXAMPLE 1" width="100%">
      <p>Examples of the original 31 cm WorldView-3 image and the 9 cm super-resolution result in comparison to the ground-based photos and map of the bar-pattern target. WorldView-3 image courtesy of Maxar 2020. Data provided by the European Space Agency.</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/EO-HR-SRR-2.png" alt="EO HR SRR EXAMPLE 2" width="100%">
      <p>Examples of the 31 cm WorldView-3 image crops and the corresponding super-resolution results showing small buildings over a site in Baotou, China. WorldView-3 image courtesy of Maxar 2020. Data provided by the European Space Agency.</p>
    </td>
  </tr>
</table>

**Super-resolution restoration of high-resolution multi-spectral satellite images.**

In contrast to “photo-enhancing” super-resolution (SR/SRR) tasks, the desired SRR outputs of remote sensing applications are fundamentally different. In remote sensing applications, higher signal-to-noise ratio (SNR), minimised artefacts, sharper edges and object outlines, and ultimately, the higher image effective resolution, are much more desirable in comparison to “re-creating” high-frequency textures and/or objects. The original design of the popular photo-SR networks are based on the idea that human vision does not care if the generated high-frequency textures are not strictly correlated with the ground truth as long as they look realistic. Such generated high-frequency textures can significantly improve the “perceptual sharpness” but are considered artefacts in remote sensing or scientific applications. For example, satellite image users probably do not want a synthetic map even it looks extremely real. Therefore, we consider perceptual quality-driven SRR techniques are not suitable to be used directly in any remote sensing applications. In this work, we demonstrate our inhouse multi-spectral deep learning models for remote sensing image super-resolution restoration that improves the image effective resolution but with minimised "photo-realistic" artefacts.

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/EO-MR-SRR.png" alt="EO MR" width="100%">
      <p>An example of the 10 m/pixel Sentinel-2 “true” colour image and the 3.44 m/pixel SRR results over a geo-calibration site at Baotou, China.</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/EO-MS-SRR.png" alt="EO MS SRR" width="100%">
      <p>An example of intercomparisons of all spectral bands of our SRR product against the original Sentinel-2 L2A surface reflectance product.</p>
    </td>
  </tr>
</table>

**Multi-Image Cloud Detection and Tracking of Satellite VIS and TIR Images.**

Automated masking and tracking of the ever-changing cloud distributions captured by the Earth observation satellites are of fundamental importance to many remote sensing applications. For surface monitoring and land feature studies, clouds need to be masked and excluded from subsequent processing and analysis. On the other hand, for retrievals of geophysical parameters and atmospheric studies, clouds need to be tracked and extracted for subsequent processing and analysis. Although manual digitisation or using interactive cloud labelling tools can obtain fairly accurate cloud masks from still images, it requires a lot of time and resources, and is not considered effective for continuous cloud masking and tracking tasks. In this work, we use our in-house deep learning based 3D optical flow pipeline to track and compute the cloud motion vectors, and subsequently using a 3D geometry based automated cloud detection technique to produce accurate cloud masks from either single-camera continuous observation, multi-camera simultaneous observation, and/or multi-camera non-simultaneous observation.

An example of the derived cloud motion vectors and scene predictions from input GOES-17 B02 (red visible) images (7 June 2021 22.00-23.00 GMT) using deep learning based 3D optical flow.

<style>
.table {
  display: table;
  width: 100%;
  table-layout: fixed;
}

.table-row {
  display: table-row;
}

.table-cell {
  display: table-cell;
  width: 33.33%;
  vertical-align: top;
  padding: 0 10px;
}

.table-cell img {
  width: 100%;
  height: auto;
}
</style>

<div class="table">
  <div class="table-row">
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-1-1-compressed.gif" alt="3D OF 1-1" />
      <p>Input GOES-17 band 02 image</p>
    </div>
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-1-2-compressed.gif" alt="3D OF 1-2" />
      <p>Cloud tracking and motion vectors</p>
    </div>
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-1-3-compressed.gif" alt="3D OF 1-3" />
      <p>Predicted scenes from the derived cloud motion vectors</p>
    </div>
  </div>
</div>

An example of the derived cloud motion vectors and scene predictions from input GOES-16 B13 (thermal infrared) images (7 June 2021 22.00-23.00 GMT) using deep learning based 3D optical flow.

<div class="table">
  <div class="table-row">
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-2-1-compressed.gif" alt="3D OF 1-1" />
      <p>Input GOES-16 band 13 image</p>
    </div>
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-2-2-compressed.gif" alt="3D OF 1-2" />
      <p>Cloud tracking and motion vectors</p>
    </div>
    <div class="table-cell">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/of-2-3-compressed.gif" alt="3D OF 1-3" />
      <p>Predicted scenes from the derived cloud motion vectors</p>
    </div>
  </div>
</div>


**Automated multi-resolution image co-registration of Mars orbital datasets.**

Automated multi-resolution HiRISE (25 cm), CaSSIS (4.5 m), CTX (6 m) and HRSC (12.5 m) image co-registration is performed using global least squares fitting and mutual shape adapted feature matching algorithms. The co-registration accuracy achieved is up to the subpixel level of the coarser layer. 

![CTX Coreg](https://surrey-ai-imaging-limited.github.io/demos/coreg-ctx.png)

Examples of the input CTX images, before CTX-to-HRSC image co-registration (1st row) and after CTX-to-HRSC image co-registration (2nd row). The example CTX images are in side-by-side views with the corresponding HRSC MC-11W level 5 orthorectified image mosaic (1st and 3rd columns) and in side-by-side views with the neighbouring CTX images (2nd and 4th columns).

![HiRISE Coreg](https://surrey-ai-imaging-limited.github.io/demos/coreg-hirise.png)

Examples of the input HiRISE images, before HiRISE-to-CTX image co-registration (1st row), and after HiRISE-to-CTX image co-registration (2nd row). The example HiRISE images are in side-by-side views with the corresponding CTX images (HRSC co-registered; 1st and 3rd columns) and in side-by-side views with the neighbouring HiRISE images (2nd and 4th columns).


**Automated dynamic feature tracking.**

To be added.

**Large area high-resolution 3D mapping of the lunar surface.**

Here we demonstrate using our in-house deep learning-based 3D modelling system to produce a large area high-resolution (260 × 209 km² at 1 m/pixel) digital terrain model (DTM) mosaic from the Lunar Reconnaissance Orbiter Camera (LROC) Narrow Angle Camera (NAC) images, over the Chang’E-4 landing site at Von Kármán crater. The resultant DTM mosaic is co-aligned with the Chang’E-2 (CE-2) and the Lunar Orbiter Laser Altimeter (LOLA) – SELenological and Engineering Explorer (SELENE) blended SLDEM, providing high spatial and vertical congruence. 

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/moon-1.png" alt="moon-1" width="100%">
      <p>The resultant 1 m LROC NAC DTM mosaic (colourised by height and hillshaded).</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/moon-2.png" alt="moon-2" width="100%">
      <p>An example of the zoom-in views of the NASA PDS LROC NAC image (NAC_DTM_CHANGE4_M1303619844_140CM.IMG), the NASA PDS LROC NAC DTM (NAC_DTM_CHANGE4_E458S1775), and our LROC NAC DTM. The DTMs are shown as colourised heights (top) and shaded relief images (bottom).</p>
    </td>
  </tr>
</table>
<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/moon-3.png" alt="moon-3" width="100%">
      <p>An example of the zoom-in views of the NASA PDS LROC NAC image (NAC_DTM_CHANGE4_M1303619844_140CM.IMG), the NASA PDS LROC NAC DTM (NAC_DTM_CHANGE4_E458S1775), and our LROC NAC DTM. The DTMs are shown as colourised heights (top) and shaded relief images (bottom).</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/moon-4.png" alt="moon-4" width="100%">
      <p>An example of the zoom-in views of the NASA PDS LROC NAC image (NAC_DTM_CHANGE4_M1303619844_140CM.IMG), the NASA PDS LROC NAC DTM (NAC_DTM_CHANGE4_E458S1775), and our LROC NAC DTM. The DTMs are shown as colourised heights (top) and shaded relief images (bottom).</p>
    </td>
  </tr>
</table>

**Wide baseline stereo reconstruction of ground-based Mars rover imagery.**

In this work, we collect multi-view imaging data from ground-level robotic and orbital sensors covering the past and on-going Mars rover missions, e.g., Spirit, Opportunity, Curiosity, and process them into a coherent set of co-registered 3D imaging products using our inhouse photogrammetric and structure from motion stereo reconstruction pipelines. We generate and fuse multi-resolution ground-level 3D models from different instruments onboard the same rover, e.g., Mastcam and Navcam from Curiosity, Pancam and Navcam from Spirit and Opportunity, using a combination of traditional computer vision algorithms, including subpixel-scale feature matching, region growing, bundle adjustment, and 3D point cloud co-alignment. These digitised multi-resolution 3D ground-level products enable the “virtual geologist” to perform close-up visual analysis of key Mar surface features, e.g., sedimentary layers, bedrocks, etc., and make measurements (e.g., distance, dip and slope) at the highest possible level of details and accuracy.

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/rover-3.png" alt="rover-3" width="100%">
      <p>Input Mastcam images from the NASA Mars Science Laboratory's curiosity rover (at Solar day 131 – Gillespie Lake).</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/rover-4.png" alt="rover-4" width="100%">
      <p>Output Mastcam 3D model using 8 input Mastcam images and a separately produced Navcam 3D model as reference baseline.</p>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/rover-1.gif" alt="rover-1" width="100%">
      <p>3D reconstruction results of the Navcam (greyscale) and Mastcam (RGB colour) images onboard the Mars Science Laboratory's Curiosity rover (at Solar day 120 – Shaler).</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/rover-2.gif" alt="rover-2" width="100%">
      <p>3D reconstruction results and examples of 3D distance measurements of the Mastcam images onboard the Mars Science Laboratory's Curiosity rover (at Solar day 131 – Gillespie Lake).</p>
    </td>
  </tr>
</table>

# Services

- Software 
- Data processing
- Consultancy


# Collaborations 

UCL, NASA JPL, Joanneum Research (Austria)


# Contact

General: saiil.info.general@gmail.com
Technical collaboration: yu.tao@saiil.co.uk


# Social Media

- LinkedIn
- Twitter
- Facebook

To be added.
