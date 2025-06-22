# black---white-to-colour-image
This project colorizes black-and-white images using a pretrained Caffe model with OpenCV. Just run the script with an input image, and it outputs a realistic color version.

# Image Colorization with Pretrained Caffe Model

This project demonstrates automatic image colorization using a deep learning model trained in Caffe. It utilizes OpenCV and a pretrained model to convert black-and-white images into colorized versions.

## 📁 Project Structure

```
.
├── b2w.py                                  # Main Python script to run the colorization
├── pts_in_hull.npy                         # Cluster centers used for ab color prediction
├── colorization_deploy_v2.prototxt        # Network architecture (download from description)
├── colorization_release_v2.caffemodel     # Pretrained weights (download from description)
```

> 📥 **Note:** Download the `.prototxt` and `.caffemodel` files from the links provided in the description.

## 🧠 Model Information

- **Model**: Colorful Image Colorization (Zhang et al.)
- **Framework**: Caffe
- **Paper**: [Colorful Image Colorization (ECCV 2016)](https://arxiv.org/abs/1603.08511)
- **Pretrained Weights**: Provided by the authors.

## 📦 Requirements

- Python 3.x
- OpenCV (with contrib modules)
- NumPy

### 🔧 Install dependencies:

```bash
pip install opencv-python opencv-contrib-python numpy
```

## 🚀 Usage

```bash
python b2w.py --input path_to_bw_image.jpg --output path_to_save_result.jpg
```

`b2w.py`:
- `colorization_deploy_v2.prototxt`
- `colorization_release_v2.caffemodel`
- `pts_in_hull.npy`

## 📸 Sample Results

Grayscale input images are transformed into visually plausible colored images using the pretrained deep learning model.

## 📌 Credits

- Based on the work by **Richard Zhang et al.**
- Colorization technique from the paper: *Colorful Image Colorization*
