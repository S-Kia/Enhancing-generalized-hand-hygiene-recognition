# Enhancing Generalized Hand Hygiene Recognition

## Objectives

1. **Generalize Recognition Across Individuals:** Develop methods to create a system that works effectively for a broad range of users.
2. **Optimize Recognition with a Single Camera:** Ensure high performance using only one camera to facilitate easy application in hand-washing analysis.
3. **Develop and Evaluate:** Utilize different methods to generalize the training model and assess their performance.

---

## Credit

Original dataset and inspiration from [SunnySideUp11/Hand-Hygiene-ICU](https://github.com/SunnySideUp11/Hand-Hygiene-ICU.git).

---

## Data Structure

```plaintext
.
├── code
│   └── ...
└── data
    ├── landmark
        ├── 1 folder (one for each view)
        ├── 8 folders (one for each person)
        ├── 7 CSV files (one for each handwashing step)
```

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/S-Kia/Enhancing-generalized-hand-hygiene-recognition.git
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. Open the `Generalized_hand_hygiene_recognition.ipynb` notebook.
2. The notebook is divided into two independent sections:
   - **Section 1:** For training the model.
   - **Section 2:** For testing on a camera feed or image (default = camera).

---

## Note

This project uses data from only one view. If you wish to apply all the available data, you can download the complete dataset from [SunnySideUp11/Hand-Hygiene-ICU](https://github.com/SunnySideUp11/Hand-Hygiene-ICU.git).

---

## Limitations

1. **Environmental Variations:** Issues such as motion blur and soap interference cannot be detected by MediaPipe.
2. **Real-Time Response:** The webcam application may respond slowly because it normalizes data in real time with dimensions of (7185, 126).
