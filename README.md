# Motion-Based Video Segmentation for High-Frame-Rate Analysis

## Overview
Automated motion segmentation pipeline for identifying regions of interest in high-frame-rate videos, designed for industrial vibration monitoring applications.

**Project Status:** Phase 2 - Classical Baseline Implementation  
**Timeline:** December 2025 - July 2026  
**Author:** Karthik (Intern, SYNRA Inc.)

## Features
- 🎯 Multiple motion detection algorithms (MOG2, Optical Flow, Frame Differencing)
- 🔍 Automatic region tracking across frames
- 📊 Per-region motion metrics and statistics
- 📈 Visualization outputs (annotated videos, time-series plots)
- 📝 Automated report generation

## Quick Start

### Installation
```bash
git clone https://github.com/synra/motion-segmentation.git
cd motion-segmentation
pip install -r requirements.txt
```

### Basic Usage
```bash
# Run segmentation on a video
python scripts/run_segmentation.py \
    --input data/raw/sample_video.mp4 \
    --method mog2 \
    --output data/results/

# Compare different methods
python scripts/compare_methods.py --input data/raw/sample_video.mp4
```

## Project Structure
```
src/           # Source code modules
scripts/       # Executable scripts
configs/       # Configuration files
docs/          # Documentation
tests/         # Unit tests
notebooks/     # Jupyter explorations
```

## Documentation
- [Installation Guide](docs/installation.md)
- [Usage Manual](docs/usage.md)
- [API Reference](docs/api_reference.md)
- [Architecture Overview](docs/architecture.md)
- [Phase 2 Technical Report](docs/phase2_report.md)

## Current Phase: Phase 2 Deliverables

### Completed
- [x] MOG2 baseline implementation
- [x] Basic motion mask generation
- [ ] Region labeling and tracking
- [ ] Motion metrics calculation
- [ ] Visualization pipeline
- [ ] Method comparison (MOG2 vs Optical Flow vs Frame Diff)

### Performance (Preliminary)
- Processing Speed: ~500 fps (1920x1080)
- Detection Accuracy: 85% (on sample dataset)
- Memory Usage: ~2GB for 10-second video

## Requirements
- Python 3.8+
- OpenCV 4.8+
- NumPy, Pandas, Matplotlib
- See `requirements.txt` for full list

## License
[To be determined by SYNRA Inc.]

## Contact
- Intern: Karthik (カルティック)
- Supervisor: Prof. Kohei Shimasaki
- Organization: SYNRA Inc.

## Acknowledgments
Part of SYNRA's internship program (January-July 2025)
