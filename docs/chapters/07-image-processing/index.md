---
title: "Chapter 7: Image Processing & Orthomosaic Generation"
description: "Transforming hundreds of raw drone images into georeferenced orthomosaics — from stitching algorithms and GSD calculation to cloud processing platforms."
---

# Chapter 7: Image Processing & Orthomosaic Generation

!!! info "Learning Objectives"
    After completing this chapter, you will be able to:
    - **Describe the photogrammetric pipeline** from raw images to georeferenced orthomosaic output
    - **Calculate and optimize ground sampling distance** (GSD) for turf analytics applications
    - **Compare processing platforms** including DJI Terra, Pix4D, and WebODM for turf-specific workflows
    - **Evaluate cloud vs. local processing tradeoffs** for operational efficiency and data security

## Key Concepts

1. Photogrammetric stitching algorithms
2. Structure from Motion (SfM) reconstruction
3. Ground Sampling Distance (GSD) calculation
4. Georeferencing and coordinate systems
5. Orthomosaic generation pipeline
6. DJI Terra processing workflow
7. Pix4Dfields for agriculture/turf
8. WebODM open-source processing
9. Cloud processing platforms and APIs
10. Point cloud generation and DSM extraction
11. Radiometric calibration in processing
12. Processing quality settings and tradeoffs
13. Export formats (GeoTIFF, KML, Shapefile)
14. Batch processing for temporal datasets
15. Quality assessment and error detection

## Summary

A single golf course survey mission generates 300-800 individual images that must be transformed into a seamless, geometrically accurate orthomosaic before any meaningful analysis can occur. This transformation — photogrammetric processing — uses Structure from Motion algorithms to identify matching features across overlapping images, reconstruct the three-dimensional geometry of the scene, and project the combined imagery onto a georeferenced coordinate plane. The quality of this processing directly determines the accuracy of every subsequent vegetation index calculation and health assessment.

Ground Sampling Distance (GSD) — the real-world size represented by a single pixel — is the fundamental resolution metric for aerial turf analytics. At 220 feet AGL with the M3M's RGB sensor, GSD is approximately 1.5 cm/pixel; multispectral bands achieve roughly 3 cm/pixel. This resolution is sufficient to detect stress patterns at the individual green or fairway zone level, though not individual plant resolution. Understanding GSD helps operators and superintendents set appropriate expectations for what aerial analytics can and cannot resolve.

The processing platform landscape offers distinct tradeoffs. DJI Terra provides tight integration with DJI hardware and straightforward multispectral processing but limited analytical tools. Pix4Dfields delivers agriculture-optimized workflows with built-in vegetation index generation and zone management. WebODM offers an open-source alternative with full processing capability and no per-image licensing costs, at the expense of requiring more technical setup. This chapter evaluates each platform's strengths for turf analytics workflows and provides configuration guidance for optimal results.

*Full chapter content will be generated using the YODA pipeline.*
