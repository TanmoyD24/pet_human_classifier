# Pet vs Human Image Classifier  
Repository: [TanmoyD24/pet_human_classifier](https://github.com/TanmoyD24/pet_human_classifier)

## 📖 Project Overview  
This project is an image-based classifier that predicts whether a given image contains a **pet** or a **human**.  
It demonstrates the workflow of:  
- dataset preparation (images labelled “pet” vs “human”)  
- training a deep learning classification model  
- running inference on new images  
- (optionally) evaluating performance metrics  

## 🧩 Key Features  
- Simple binary classifier (pet vs human)  
- Pre-processing for images: resizing, normalization, augmentation  
- Model built with [insert framework here: e.g., TensorFlow / PyTorch / Keras]  
- Supports inference of single images or batch processing  
- (Optional) Checkpointing, logging, ▢ visualization of results  

## 📂 Repository Structure  
pet_human_classifier/
├── data/
│ ├── train/ ← training images (subfolders: pet/, human/)
│ ├── val/ ← validation images
│ └── test/ ← test images
├── models/ ← saved model checkpoints
├── notebooks/ ← Jupyter notebooks (e.g., training, explorations)
├── src/ ← source code (pre-processing, model definition, inference)
├── inference.py ← script for running inference on new images
├── train.py ← script for training the model
├── requirements.txt ← list of required Python packages
└── README.md ← (this file)


## 🛠 Installation & Setup  
1. Clone the repo:  
   ```bash
   git clone https://github.com/TanmoyD24/pet_human_classifier.git  
   cd pet_human_classifier  
2. Create/activate a virtual environment (optional but recommended):
   python3 -m venv venv  
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`  
   pip install -r requirements.txt  
3. Download or prepare your dataset into the data/ folder as per the structure above

📊 Evaluation & Metrics

After training/evaluation you should report key metrics such as:

Accuracy

Precision, Recall, F1-score (for each class)

Confusion Matrix

(Optional) ROC Curve & AUC
Include details of your validation/test split and any caveats (class imbalance, image quality variation, etc).

🔍 Model / Architecture Details

Describe here:

Which model architecture you used (e.g., ResNet50/ MobileNet / custom CNN)

Input image size (e.g., 224×224)

Pre-processing steps (normalization, augmentation: flip, rotation, zoom)

Any transfer learning used or training from scratch

Loss function, optimizer, learning rate

Number of parameters, training time, hardware used

How many classes (2: pet / human) and how class labels are encoded

✅ Results & Findings

Summarise your experiment results:

Training accuracy & loss over epochs

Validation accuracy & loss

Best model checkpoint performance on test set

Sample predictions with images (good and challenging cases)

Any failure/bias cases observed

⚠️ Limitations & Future Work

Dataset limitations: e.g., limited variety of pets/humans, lighting/pose issues

Model limitations: over-fitting, generalisation to unseen types

Potential improvements:

More classes (e.g., dog vs cat vs human)

Better augmentation / domain adaptation

Real-time inference / mobile deployment

Explainability (Saliency maps, Grad-CAM)

Larger dataset, improved annotation

🧪 Contributing

If you’d like to contribute:

Please fork the repository and create a pull request.

Ensure your changes include tests (if applicable) and maintain code style.

Update this README with any new features or dependencies.