# Face Verification Benchmark for eKYC

## Overview

This project is a Python-based benchmark framework for evaluating face verification models in an eKYC-like scenario.

The goal was to compare multiple face recognition models and select a suitable candidate for an eKYC MVP based on accuracy, security, runtime performance, model size, and deployment readiness.

## Problem

In an eKYC flow, the system needs to verify whether a user’s captured face matches an official reference image.

Choosing a face verification model only based on accuracy is not enough. For a financial or identity verification use case, the model must also be evaluated based on false accepts, false rejects, runtime performance, and deployment constraints.

## Approach

The benchmark pipeline includes:

- Face detection
- Face validation
- Face alignment
- Face embedding extraction
- Cosine similarity comparison
- Threshold-based match decision
- Evaluation report generation

## Models Evaluated

The following models were evaluated:

- ArcFace
- MobileFaceNet
- GhostFaceNet
- EdgeFace
- FaceNet
- AdaFace

## Dataset

The initial benchmark was performed on LFW, a pair-based face verification dataset.

The evaluation used 6,000 requested pairs with a balanced sampling strategy.

## Metrics

The benchmark compared models using:

- Accuracy
- FAR — False Accept Rate
- FRR — False Reject Rate
- EER — Equal Error Rate
- TAR@FAR
- FPS
- Average processing time per pair
- Model size
- Weighted decision score

## Result Summary

EdgeFace achieved the best overall balance between accuracy, security, performance, and deployment readiness.

| Rank | Model | Accuracy | FAR | FRR | FPS | Size MB | Weighted Score | Final Decision |
|---:|---|---:|---:|---:|---:|---:|---:|---|
| 1 | EdgeFace | 95.28% | 0.00% | 9.45% | 1.98 | 6.94 | 73.15 | Recommended |
| 2 | GhostFaceNet | 91.95% | 0.00% | 16.12% | 2.00 | 15.46 | 71.14 | Backup |
| 3 | MobileFaceNet | 90.54% | 0.00% | 18.94% | 1.93 | 12.99 | 70.87 | Optional |
| 4 | FaceNet | 96.28% | 0.10% | 7.34% | 1.82 | 89.61 | 65.17 | Baseline |
| 5 | ArcFace | 95.33% | 0.00% | 9.35% | 1.55 | 166.31 | 63.75 | Baseline |
| 6 | AdaFace | 94.69% | 0.00% | 10.63% | 1.53 | 166.32 | 63.53 | Baseline |

## Final Recommendation

EdgeFace was selected as the initial face verification model for the eKYC MVP.

The main reasons were:

- Best overall weighted score
- Small ONNX model size
- Good accuracy
- Zero FAR at the fixed benchmark threshold
- CPU-friendly deployment profile
- Better deployment readiness compared with heavier baseline models

GhostFaceNet was kept as a lightweight backup candidate.

## Technical Stack

- Python
- ONNX Runtime
- InsightFace
- OpenCV
- NumPy
- Pandas
- Pytest
- Ruff
- Black
- Excel report generation

## Limitations

This benchmark was focused on face verification only.

The following areas require separate evaluation:

- Active liveness detection
- Passive liveness / anti-spoofing
- Real mobile camera videos
- Low-light and blur scenarios
- Pose variation
- Age variation
- Replay and spoof attacks

## Next Steps

- Integrate EdgeFace into the eKYC MVP service
- Run additional benchmarks on pose and age variation datasets
- Build a separate evaluation pipeline for active liveness
- Build a separate evaluation pipeline for passive liveness and anti-spoofing
- Validate thresholds using real eKYC-like samples
