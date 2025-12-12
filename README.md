# Survue Bike Safety Object Detection

Real-time object detection system for Survue's bike-mounted safety lights using YOLOv8 models to detect vehicles, pedestrians, and traffic signs.

## Quick Start

### Prerequisites
- Python 3.10+
- CUDA 11.0+

### Installation

```bash
git clone <repo-url>
cd survue-object-detection
pip install -r requirements.txt
```

### Running

1. Open notebook in `notebooks/`
2. Update data path:
```python
DATA_ROOT = "/path/to/your/data/FinalProject"
ANNOTATIONS_DIR = f"{DATA_ROOT}/annotations"
IMAGES_DIR = f"{DATA_ROOT}/images"
```
3. Run all cells

## Dataset

- **Images:** 500 (393 train, 107 val)
- **Annotations:** 9,787
- **Classes:** Human, Vehicle, Traffic Sign

## Output

Results saved to:
- `runs/survue_yolov8{model}/weights/best.pt` - Trained model
- `results/evaluation_metrics.json` - Performance metrics
- `results/predictions/` - Sample predictions

## Notebooks

- `Yolov8smodel.ipynb` - YOLOv8 Small
- `Yolo8mModel.ipynb` - YOLOv8 Micro 
- `YoloVn.ipynb` - YOLOv8 Nano
- `YoloVl.ipynb` - YOLOv8 Large (recommended)
