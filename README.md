# Surrey AI Imaging


# Introduction

Surrey AI Imaging Ltd. is a technology startup located in Surrey, UK that specialises in image processing and AI, particularly in the areas of planetary remote sensing and Earth observation. With extensive experience in computer vision, remote sensing, machine learning, and deep learning, the technical team at Surrey AI Imaging Ltd. possesses a comprehensive understanding of image processing algorithms, deep learning models, and their applications to solve complex and challenging problems in planetary and Earth remote sensing. Our expertise encompasses the following applications:

- Satellite image and video super-resolution restoration, including restoration from lower-resolution (>500 m) to higher-resolution (20 m – 4 m) and ultra-high-resolution (30 cm – 1 m) imagery and videos, as well as from visible bands (panchromatic and RGB) to multispectral bands.
- Photogrammetry, photoclinometry, structure from motion and monocular height estimation based 3D reconstruction (i.e., digital terrain modelling, topographic mapping).
- Subpixel-scale 3D reconstruction using coupled deep learning based image super-resolution and monocular height estimation. 
- Satellite image shadow detection, deshading and reshading using deep learning.
- Satellite image matching, multi-resolution image co-registration and mosaicing.
- Optical flow and 3D scene flow based feature and scene tracking, such as cloud masking and cloud motion vector retrieval.
- Object and ground feature detection, segmentation, classification, and tracking for buildings, cars, airplanes, trees, people on the Earth, and rocks, craters, layers, and dynamic surface features on planetary surfaces.
- GPU optimisations and onboard "smart-sattelite" solutions of remote sensing applications.

Surrey AI Imaging Ltd. is dedicated to providing innovative and cutting-edge solutions to address the challenges faced in the field of satellite imaging and planetary remote sensing.


# People
<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/pictures/crop-jiao.jpg" alt="Kejing Zhu" width="100%">
      <p>Kejing Zhu: Director and Company Secretary</p>
      <p>Kejing Zhu brings Surrey AI Imaging Limited her leadership experience in fast growth technology start-ups of various sizes and across different industries including new media, data analysis, advertising business, remote sensing applications, education and outreach. She was previously Director of Cross Culture Communications Ltd. and has a background in accounting and marketing communications. Kejing has a M.A. degree in Interpreting from Middlesex University, London.</p>
    </td>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/pictures/crop-dou.jpg" alt="Yu Tao" width="100%">
      <p>Dr. Yu Tao, Ph.D.: Technical Director</p>
      <p>Yu Tao has extensive experience in the remote sensing industry and plantary science with a unique mix of expertise in computer vision, machine learning and deep learning, planetary remote sensing and Earth observation systems as well as software engineering. He has a long track record of successfully leading complex software engineering projects and achieving technology breakthroughs on challenging tasks. Prior to his work with Surrey AI Imaging Ltd. Yu was a senior research scientist at the University College London where he led and developed cutting-edge AI and computer vision software for plantary remote sensing and Earth observation applications. Yu has served as the lead researcher and software engineer in three European Commission 7th Framework – Space projects and as a co-investigator and project manager in two UK Space Agency Centre for Earth Observation and Instrumentation (CEOI) funded Earth observation initiatives. Yu holds a Ph.D. in Planetary 3D Imaging from the University College London and is currently serving as an Honorary Research Fellow at the same institution.</p>
    </td>
  </tr>
</table>


# Our work

**Super-3D: subpixel-scale 3D reconstruction from Mar remote sensing imagery using deep learning based image super-resolution and monocular height estimation.**

High-resolution digital terrain models (DTMs) play an important role in studying the formation processes involved in generating a modern-day planetary surface such as Mars. However, it has been a common understanding that DTMs derived from a particular imaging dataset can only achieve a lower, or at the best, similar effective spatial resolution compared to the input images, due to the various approximations and/or filtering processes introduced by the photogrammetric and/or photoclinometric pipelines. With recent successes in deep learning techniques, it is now become feasible to improve the effective resolution of an image using super-resolution restoration (SRR) networks, retrieving pixel-scale topography using single-image DTM estimation (SDE) networks, and subsequently, combine the two techniques to produce subpixel-scale topography from only a single-view input image. In this work, we demonstrate with the UCL MARSGAN SRR [1] and the MADNet SDE [2] systems to produce single-input-image-based DTMs at subpixel-scale spatial resolution [3] using the 4 m/pixel ESA Trace Gas Orbiter Colour and Stereo Surface Imaging System (CaSSIS) “PAN” band images and the 25 cm/pixel NASA Mars Reconnaissance Orbiter High Resolution Imaging Science Experiment (HiRISE) “RED” band images.

[1] Tao, Y.; Conway, S.J.; Muller, J.-P.; Putri, A.R.D.; Thomas, N.; Cremonese, G. Single Image Super-Resolution Restoration of TGO CaSSIS Colour Images: Demonstration with Perseverance Rover Landing Site and Mars Science Targets. Remote Sens. 2021, 13, 1777. 
[2] Tao, Y.; Muller, J.-P.; Xiong, S.; Conway, S.J. MADNet 2.0: Pixel-Scale Topography Retrieval from Single-View Orbital Imagery of Mars Using Deep Learning. Remote Sens. 2021, 13, 4220.
[3] Tao, Y.; Xiong, S.; Muller, J.-P.; Michael, G.; Conway, S.J.; Paar, G.; Cremonese, G.; Thomas, N. Subpixel-Scale Topography Retrieval of Mars Using Single-Image DTM Estimation and Super-Resolution Restoration. Remote Sens. 2022, 14, 257.

<table>
  <tr>
    <td style="width:50%; height:300px;">
      <img src="https://surrey-ai-imaging-limited.github.io/demos/Super-3D.png" alt="Super-3D" width="100%">
      <p>Example of CaSSIS Super-3D products for Oxia Planum: the landing site of the ESA ExoMars Rosalind Franklin rover. Upper-left: input 4 m TGO CaSSIS image; Upper-right: output 1 m CaSSIS super-resolution resolved image; Lower-left: output 8 m CaSSIS 3D model using monocular height estimation; Lower-right: output 2 m CaSSIS Super-3D model using coupled image super-resolution and monocular height estimation.</p>
    </td>
    <td style="width:50%; height:300px;">
      <iframe width="300" height="200" src="https://www.youtube.com/embed/ulONddVFiOw?list=PL4kOs9mVzcpYiJ1YNd4g5HIdsj3FOQ0Rm" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>      
      <p>subpixel-scale 3D reconstruction from Mar remote sensing imagery explained.</p>
    </td>
  </tr>
</table>

**Super-Resolution Restoration (SRR) of ultra-high-resolution satellite images.**

Increasing the spatial resolution of spaceborne imagery and video using ground-based processing, or, where feasible, onboard a smart satellite, allows greater amounts of information to be extracted about the scene content. Such processing is generally referred to as super-resolution restoration (SRR). SRR techniques are applicable to images and videos without the usual increased costs and mass, associated with increased bandwidth or larger/heavier optical components, normally required for achieving higher resolution. In particular, enhancing the ultra-high spatial resolution Earth observation (EO) images, or high definition (HD) videos, is an active driver for many applications in the fields of agriculture, forestry, energy and utility maintenance and urban geospatial intelligence. The ability to further improve 30 cm/80 cm EO images and videos into 10 cm/30 cm resolution SRR images and videos will allow EO analytics to be performed in transformative ways.



# Services

- Software 
- Data processing
- Consultancy


# Collaborations 

UCL, NASA JPL, Joanneum Research (Austria)


# Contact

Technical and collaboration: yu.tao@ucl.ac.uk


# Social Media

- LinkedIn
- Twitter
- Facebook

