# caribou-detection-system

The problem that I am attempting to solve:
https://www.adfg.alaska.gov/index.cfm?adfg=wildlifenews.view_article&articles_id=869

The Caribou Detection System (CDS) is an open-source application designed to automatically detect and count caribou (and likely future species such as Dall sheep) from stitched together, high-resolution aerial photographs. The goal is to reduce the labor-intensive process of manual counting to simply ensuring the quality of the model's analysis.

This project is intended for state wildlife agencies, researchers, conservation teams, and anyone managing large-scale wildlife populations using aerial surveys.

# Planned features
1. Load large aerial images (including GeoTIFFs)
2. Automatic detection of caribou using a tuned YOLOv8 model
3. GPU-accelerated inference (CUDA, if available)
4. Tiling system to handle extremely large 100–400 MP images
5. Display detection results in an interactive desktop GUI
6. Export detection counts and geospatial metadata

Initial implementation will be in Python. It will eventually be completely phased out or reduced to a minimal amount by C++ or potentially Rust.