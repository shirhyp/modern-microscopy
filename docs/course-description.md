---
title: Course Description for EE 5940 Advanced Topics in Modern Microscopy Techniques
description: A detailed course description for EE 5940 Advanced Topics in Modern Microscopy Techniques including overview, topics covered and learning objectives in the format of the 2001 Bloom Taxonomy
quality_score: 100
---

# EE 5940 — Advanced Topics in Modern Microscopy Techniques

**Title:** Advanced Topics in Modern Microscopy Techniques (EE 5940, Special Topics in Electrical Engineering I)

**Institution:** University of Minnesota, Department of Electrical and Computer Engineering

**Instructor:** Hye Yoon Park

**Target Audience:** Graduate students and advanced undergraduates in electrical engineering, biomedical engineering, physics, and related fields who build, use, or analyze data from optical microscopes in their research.

**Prerequisites:** EE 3601 (Transmission Lines, Fields, and Waves) or an equivalent course in electromagnetics, or the instructor's permission. Students should be comfortable with Maxwell's equations, plane waves, complex phasors, Fourier transforms, and basic linear algebra and probability. Some programming experience (Python or MATLAB) is helpful for the computational imaging topics.

**Format:** Two 75-minute in-person lectures per week (also available through UNITE), three homework assignments, and a term project in which each student presents and reports on a recent research paper about a modern optical microscopy technique.

**References:** Jerome Mertz, *Introduction to Optical Microscopy*; Douglas B. Murphy and Michael W. Davidson, *Fundamentals of Light Microscopy and Electronic Imaging*.

## Course Overview

Optical microscopes have changed from simple magnifiers into precision instruments that combine lasers, engineered optics, fast scanners, sensitive electronic detectors, and heavy computation. This course takes an engineering view of that instrument. It starts from electromagnetic wave theory and diffraction, and asks how those physical principles set the resolution, contrast, speed, and signal-to-noise ratio (SNR) a microscope can achieve. It then follows the light through the system: illumination and detection paths, objective and relay optics, contrast-generating hardware, image sensors and their noise, sampling and digitization, and finally the computational pipelines that turn raw pixels into quantitative measurements.

Current research in light microscopy is discussed throughout, on top of a solid understanding of image formation in conventional microscopes. Laser-scanning and nonlinear systems, adaptive optics for imaging through scattering tissue, deconvolution and denoising, quantitative image analysis, and machine learning for "smart" microscopes that control themselves in real time are all covered as engineering problems with measurable trade-offs.

The course matters because modern biology, medicine, materials science, and semiconductor inspection depend on microscopes that push physical limits, and the people who design, choose, and operate those instruments need to understand them from first principles. In the term project, each student reads a recent research paper on a modern optical microscopy technique, explains its light path and key components, judges its performance and limitations against other techniques, and presents it to the class. This builds the skill of critically reading the microscopy literature, which every researcher in the field needs.

## Main Topics Covered

1. **Foundations of optical system design.** Wave optics; scalar diffraction theory (Huygens–Fresnel, Fraunhofer and Fresnel diffraction); the Fourier-optics view of imaging; the point spread function (PSF) and optical transfer function (OTF); numerical aperture and resolution criteria (Abbe, Rayleigh, Sparrow); coherent versus incoherent imaging; engineering and measuring the PSF. Comparison with electron microscopy (resolution limits, sample requirements) and correlative light and electron microscopy (CLEM).
2. **Geometric optics in instrumentation.** Ray optics, imaging conditions, and ray-transfer matrices; Köhler and critical illumination; design of illumination and detection paths, including epi-fluorescence paths with excitation filters, dichroic mirrors, and emission filters; objective lens physics (immersion media, working distance, aberration correction, cover-glass correction); infinity-corrected systems, tube lenses, and relay optics; conjugate planes, pupils, and field stops.
3. **Advanced photodetection and sensor electronics.** Photon statistics; quantum efficiency; noise sources (shot, read, dark, clock-induced, and excess noise); SNR models; sCMOS, CCD, EMCCD, photomultiplier tubes (PMT), avalanche photodiodes (APD), and hybrid detectors; gain, dynamic range, and camera calibration.
4. **Hardware implementation of contrast.** Wavefront engineering for brightfield, darkfield, phase contrast, differential interference contrast (DIC), polarization microscopy, and interference-based and quantitative phase imaging; fluorescence contrast and its optical requirements.
5. **Digital image formation and sampling.** The Nyquist–Shannon sampling theorem applied to microscopy; matching pixel size to optical resolution; aliasing; bit depth and quantization; frame rate, field of view, and data rate; high-bandwidth data acquisition, storage, and management.
6. **Nonlinear and scanning systems.** Laser-scanning architectures; confocal pinholes and optical sectioning; galvanometric, resonant, and acousto-optic scanners; scan lenses and scan geometry; pulsed lasers and two-photon and other nonlinear excitation; nonlinear optical pathways and detection.
7. **Adaptive optics and wavefront control.** Optical aberrations and Zernike polynomials; aberrations from samples and scattering media; wavefront sensing (direct and sensorless); deformable mirrors and spatial light modulators (SLM); correction strategies for deep imaging.
8. **Computational imaging I: restoration.** Image formation as a linear forward model; the mathematical foundations of deconvolution (inverse and Wiener filtering, Richardson–Lucy, regularization); noise models and denoising; software-based aberration correction.
9. **Computational imaging II: quantitative analysis.** Image preprocessing and background correction; automated feature extraction; segmentation; particle localization and object tracking; spatial statistics for large-scale datasets; reproducible analysis pipelines.
10. **Data-driven and smart microscopy.** Machine learning (deep learning) for image restoration, segmentation, and classification; validation and failure modes of learned models; real-time automated system control and adaptive acquisition ("smart microscopy").
11. **Current research techniques (term project).** Recent advances in modern optical microscopy presented by students from the research literature, for example super-resolution, light-sheet, and other emerging methods.

## Topics Not Covered

This course focuses on optical microscopy. The following are out of scope:

- Electron microscopy as a subject in its own right (it is covered only in comparison with optical microscopy and in the context of CLEM); electron optics and electron-sample interactions are not taught in depth.
- Scanning probe microscopies such as atomic force microscopy (AFM) and scanning tunneling microscopy (STM).
- X-ray, ultrasound, and other non-optical imaging methods.
- Sample preparation, staining, and fluorophore or labeling chemistry, beyond what is needed to understand the optical requirements of an experiment.
- Biological interpretation of imaging results.
- Detailed optical lens design (for example, optimizing lens prescriptions in Zemax or Code V).
- The general theory and training of machine learning models, beyond how they are applied and validated in microscopy.

## Learning Outcomes

After completing this course, students will be able to:

### Remember
*Retrieving, recognizing, and recalling relevant knowledge from long-term memory.*

- State the Abbe, Rayleigh, and Sparrow resolution criteria and the formulas for lateral and axial resolution in terms of wavelength and numerical aperture.
- Identify the main components of an infinity-corrected microscope (light source, collector, condenser, objective, tube lens, filters, dichroic mirror, detector) and the conjugate planes in its illumination and detection paths.
- List the main noise sources of an image sensor (shot, read, dark, and excess noise) and the defining features of sCMOS, CCD, EMCCD, PMT, and APD detectors.
- Recall the Nyquist–Shannon sampling criterion and the rule for matching camera pixel size to optical resolution.
- Name the major contrast mechanisms (brightfield, darkfield, phase contrast, DIC, polarization, interference, fluorescence) and the major classes of modern techniques (confocal, multiphoton, adaptive optics, super-resolution, light-sheet).

### Understand
*Constructing meaning from instructional messages, including oral, written, and graphic communication.*

- Explain how diffraction at the objective pupil produces the point spread function, and why the optical transfer function limits which spatial frequencies reach the image.
- Explain the difference between coherent and incoherent image formation and how illumination design (Köhler versus critical illumination) affects an image.
- Describe how phase contrast, DIC, and polarization microscopy convert phase or anisotropy in a sample into intensity contrast.
- Explain how a confocal pinhole provides optical sectioning and why nonlinear (multiphoton) excitation gives intrinsic sectioning and deeper penetration in scattering tissue.
- Explain how sample-induced aberrations degrade the PSF and how adaptive optics restores it.
- Compare the resolution limits, sample requirements, and complementary strengths of optical and electron microscopy, and explain the motivation for CLEM.

### Apply
*Carrying out or using a procedure in a given situation.*

- Calculate the PSF size, lateral and axial resolution, depth of field, and magnification of a microscope configuration.
- Use ray-transfer matrices and thin-lens relations to design an illumination or relay path with specified magnification and pupil positions.
- Compute the expected SNR of a measurement for a given detector, photon flux, and exposure, and choose camera settings (gain, binning, exposure) to maximize it.
- Choose a pixel size, field of view, and frame rate that satisfy Nyquist sampling, and estimate the resulting data rate and storage requirements.
- Implement deconvolution (for example, Wiener filtering and Richardson–Lucy) and denoising on microscopy images in Python or MATLAB.
- Apply segmentation, feature extraction, and particle-tracking algorithms to extract quantitative measurements from image datasets.

### Analyze
*Breaking material into constituent parts and determining how the parts relate to one another and to an overall structure or purpose.*

- Trace the light path of a published microscope design, identify the function of each component, and locate its conjugate planes.
- Break down the noise budget of an imaging experiment to determine whether it is limited by shot noise, detector noise, or background.
- Analyze the trade-offs among resolution, imaging speed, field of view, photobleaching or phototoxicity, and SNR for a given imaging task.
- Decompose a measured wavefront or PSF into Zernike aberration modes and identify their likely physical causes.
- Distinguish real image features from artifacts caused by aliasing, aberrations, deconvolution, or machine-learning models.

### Evaluate
*Making judgments based on criteria and standards through checking and critiquing.*

- Judge which microscopy technique and detector are best for a specific scientific or engineering problem, and justify the choice with quantitative performance criteria.
- Critique a recent research paper on an optical microscopy technique, assessing its claims of resolution, speed, and SNR, and its advantages and limitations compared with other techniques.
- Assess whether a deconvolution, denoising, or machine-learning restoration result is trustworthy, using ground truth, controls, and validation metrics.
- Evaluate the cost, complexity, and benefit of adding adaptive optics, scanning hardware, or computational methods to an existing imaging system.
- Verify the accuracy of technical content and citations, including content produced with the help of AI tools.

### Create
*Putting elements together to form a coherent or functional whole; reorganizing elements into a new pattern or structure.*

- Design a microscope system (illumination path, detection path, contrast method, and detector) that meets a given set of resolution, speed, and SNR specifications.
- Build a computational pipeline that goes from raw image data through restoration and segmentation to quantitative, statistically analyzed results.
- Propose an adaptive-optics or smart-microscopy control strategy for imaging deep in scattering samples or for automated, event-driven acquisition.
- **Term project (capstone):** Write a technical report on the optical microscopy technique in an assigned recent research paper, explaining its imaging principle, light path and key components, key performance (resolution, imaging speed, SNR), and its advantages and limitations compared with other techniques.
- **Term project (capstone):** Deliver a 20-minute presentation that explains the necessary background, the technique, the significance of the paper, the interpretation of each figure, and the current status of the technique, and answer questions from the audience.
