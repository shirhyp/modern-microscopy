# Course Description Assessment

**Course:** EE 5940 — Advanced Topics in Modern Microscopy Techniques
**Assessed file:** `docs/course-description.md`
**Analyzer:** Course Description Analyzer, version 0.05
**Source:** EE 5940 syllabus, Spring 2027 (version 3, last updated November 6, 2026)

## Overall Score: 100/100

**Quality rating:** Excellent. Ready for learning graph generation.

## Detailed Scoring Breakdown

| Element | Points | Earned | Notes |
|---|---|---|---|
| Title | 5 | 5 | Course number and full title, matching the syllabus. |
| Target Audience | 5 | 5 | Graduate students and advanced undergraduates in EE, BME, physics and related fields. |
| Prerequisites | 5 | 5 | EE 3601 or equivalent electromagnetics, or instructor permission, plus the assumed math and programming background. |
| Main Topics Covered | 10 | 10 | 11 topics that follow the syllabus, each expanded into specific subtopics. |
| Topics Excluded | 5 | 5 | Seven explicit exclusions, including the syllabus limit on electron microscopy (comparison and CLEM only). |
| Learning Outcomes Header | 5 | 5 | "After completing this course, students will be able to:" |
| Remember Level | 10 | 10 | 5 specific outcomes. |
| Understand Level | 10 | 10 | 6 specific outcomes. |
| Apply Level | 10 | 10 | 6 specific outcomes. |
| Analyze Level | 10 | 10 | 5 specific outcomes. |
| Evaluate Level | 10 | 10 | 5 specific outcomes, including critiquing research papers. |
| Create Level | 10 | 10 | 3 design outcomes plus the term-project report and presentation as capstones. |
| Descriptive Context | 5 | 5 | Three-paragraph overview explaining the engineering approach and why the course matters. |
| **Total** | **100** | **100** | |

## Gap Analysis

No element scored below full points. Two points are worth noting:

- **The learning outcomes are drafted, not taken from the syllabus.** The syllabus lists topics and assignments but no Bloom-level outcomes. The outcomes were written to match the syllabus topics, the term-project report and presentation requirements, and the course's AI-use policy. The instructor should review them, because they directly shape the learning graph.
- **Some detail goes beyond the syllabus topic list.** Fluorescence (epi-fluorescence paths, filters, dichroics), confocal sectioning, Zernike modes, and named algorithms such as Wiener filtering and Richardson–Lucy were added to give the learning graph enough depth. They are standard material in the two reference books, but the instructor should remove any that the lectures will not cover.

## Improvement Suggestions

These are optional refinements, not requirements:

1. Confirm or trim the expanded subtopics in each of the 11 topics, so the learning graph matches the actual lectures.
2. If the term-project paper list is known, add the technique families it covers (for example, super-resolution, light-sheet, expansion, or label-free methods) to topic 11 so the graph includes their background concepts.
3. If homework uses a specific language or toolset (Python, MATLAB, Fiji/ImageJ, napari), name it so the computational concepts can reference it.

## Concept Generation Readiness

The description is detailed enough to generate a full learning graph:

- **Breadth:** 11 topics spanning physics (wave and geometric optics), hardware (objectives, scanners, detectors, deformable mirrors), signal processing (sampling, noise, deconvolution), and data science (analysis pipelines, machine learning).
- **Depth:** Each topic lists 5–10 named subtopics, and many of those break down further (for example, each detector type, noise source, contrast method, and scanner type is its own concept).
- **Concept types:** The outcomes call for definitions, physical principles, formulas, procedures, design trade-offs, and evaluation criteria, which gives a good mix of foundational and advanced concepts.
- **Estimated concept count:** 300–400 concepts, comfortably above the 200-concept minimum.

## Next Steps

The score is at least 85, so the course description is ready for the `learning-graph-generator` skill. Reviewing the drafted learning outcomes first is recommended.
