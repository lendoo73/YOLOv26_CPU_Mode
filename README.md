# YOLOv26 CPU Mode

A small companion project for installing Ultralytics and running YOLO26 inference on a CPU.

## Setup

Use a Python virtual environment, then install the project dependency:

```shell
python -m venv .venv
.venv\Scripts\activate
python -m pip install -r requirements.txt
```

## Run a prediction

Obtain the `yolo26l.pt` model weights from the official Ultralytics distribution and place them in this directory.
The weights are not included in this repository.

Run inference on the included `football.png` sample with CPU execution:

```shell
yolo predict model=yolo26l.pt source=football.png device=cpu
```

Ultralytics writes generated predictions under `runs/`, which is excluded from version control.

## Files

- `29-194_Install_YOLO26_in_CPU_Mode.md` — installation note from the course project.
- `football.png` — sample image.
- `requirements.txt` — Python package dependency.

The model weights and generated output files are intentionally not published. Ultralytics, its model weights,
and third-party materials remain subject to their respective licenses and terms.
