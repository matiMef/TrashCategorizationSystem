# Edge AI Waste Detection and Classification System

An end-to-end edge computing solution designed to detect, count, and categorize waste items (glass, plastic, metal, etc.) from live camera feeds.

## Architecture and Components

- **Vision Model**: A single unified model performing both object detection (bounding boxes) and multi-class waste categorization.
- **Training Environment**: High-performance local workstation powered by an RTX 5060 Ti for training and model packaging.
- **Edge Node (Radxa)**: Embedded hardware running real-time inference on camera streams, performing counting, and generating sample reports.
- **Web Application**: Dashboard for remote control, triggering snapshot actions, viewing live video feeds, and analyzing generated reports.

## Data Flow

Camera Feed (Radxa) -> Edge Model Inference (Detection and Classification) -> Snapshot and Metrics Generation -> Web Application (Reporting and Live Preview)
