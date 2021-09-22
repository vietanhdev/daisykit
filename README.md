# Daisykit SDK

**DaisyKit SDK** is the core of models and algorithms, which can be used to develop wrappers and applications for different platforms: mobile, embedded or web browsers.

**Website:** <https://daisykit.org/>.

![DaisyKit SDK](docs/images/daisykit-architecture.png)

## Environment Setup

- Install OpenCV. In Ubuntu:

```
sudo apt install libopencv-dev
```

- Install Vulkan dev. In Ubuntu:

```
sudo apt-get install -y libvulkan-dev
```

- Download [precompiled NCNN](https://github.com/Tencent/ncnn/releases), extract it (version for your development computer).

- Download all assets [here](https://drive.google.com/drive/folders/1ZAM8W4hHkV7-zmfHFjIGLAuso3QajUfW?usp=sharing) and put into `assets/` folder.

## Build and Run on PC

```
mkdir build
cd build
cmake .. -Dncnn_FIND_PATH="<path to ncnn lib>"
make
```

- Run face detection example

```
./demo_face_detector_graph
```

## Coding convention

Read coding convention and contribution guidelines [here](https://docs.daisykit.org/md_contribution.html).

## Build documentation

- Step 1: Install **doxygen** first.

- Step 2: Build the documentation:

```
cd docs
doxygen Doxyfile.in
```

- Step 3: Deploy html documentation from `docs/_build/html`.

- Step 4: Our lastest documentation is deployed at <https://docs.daisykit.org>.
