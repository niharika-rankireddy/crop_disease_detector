
# Crop Disease Detector

A cross-platform Flutter application that detects crop diseases from leaf images using an on-device TensorFlow Lite (TFLite) model. Farmers and agricultural users can capture or upload a photo of a crop leaf and instantly get a disease prediction — no internet required.

---

## Features

- Pick images from gallery or capture using camera
- On-device ML inference using TensorFlow Lite (no internet needed)
- Detects multiple crop diseases from leaf images
- Fast and lightweight — runs entirely on the device
- Supports Android, iOS, Web, Linux, macOS, and Windows (Flutter multiplatform)

---

##  Tech Stack

| Technology | Purpose |
|---|---|
| Flutter (Dart) | Cross-platform UI framework |
| TensorFlow Lite (`tflite_flutter`) | On-device ML model inference |
| `image_picker` | Camera and gallery image input |
| `image` | Image preprocessing |

---

##  Project Structure

```

crop_disease_detector/
├── android/          # Android platform files
├── ios/              # iOS platform files
├── lib/              # Main Dart source code
├── assets/
│   ├── model.tflite  # Trained TFLite classification model
│   └── labels.txt    # Disease label mappings
├── web/              # Web platform files
├── windows/          # Windows platform files
├── linux/            # Linux platform files
├── macos/            # macOS platform files
├── test/             # Unit and widget tests
└── pubspec.yaml      # Dependencies and asset config
```

---

##  Getting Started

### Prerequisites

- Flutter SDK `^3.11.1`
- Dart SDK `^3.11.1`
- Android Studio / Xcode (for mobile builds)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/niharika-rankireddy/crop_disease_detector.git
   cd crop_disease_detector
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

---

##  ML Model

The app uses a `.tflite` image classification model stored locally in the `assets/` folder.

- **Model file:** `assets/model.tflite`
- **Labels file:** `assets/labels.txt`
- **Inference:** Handled by the `tflite_flutter` package entirely on-device

> To replace the model with your own, swap `model.tflite` and `labels.txt` in the `assets/` folder and retrain using tools like [Google Teachable Machine](https://teachablemachine.withgoogle.com/) or TensorFlow's Model Maker.

---

##  Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  image_picker: ^1.0.7
  image: ^4.1.7
  tflite_flutter: ^0.11.0
  cupertino_icons: ^1.0.8
```

---

## Team

**Niharika Rankireddy** 
**Sai Krishna**
**Preethi**


