# microclimate-ml-model
Trained KNN model for classifying façade-level plant microclimates using radiation, temperature, and humidity data — used in a Grasshopper-based environmental design tool.
# Microclimate ML Model

This repository contains a trained machine learning model for classifying façade-level plant microclimate zones. The model is used within a Grasshopper plugin that helps designers identify optimal areas for green infrastructure based on local environmental conditions.

## 🌱 What It Does

The model predicts one of 20 microclimate zones based on:
- Winter and summer solar radiation
- Winter and summer temperatures
- Winter and summer relative humidity

It supports regenerative and climate-responsive architectural design by enabling early-stage decision-making for façade-integrated planting.

## 📁 Files

- `microclimate_model.pkl` – Trained K-Nearest Neighbors model
- `zone_label_encoder.pkl` – Encodes and decodes zone labels (optional)

## 🔧 How to Use

1. **Download both `.pkl` files** to a local folder (e.g., `C:/MicroclimateModel`)
2. **Run the Flask server script** provided with the Grasshopper plugin
3. **Input the model path** in Grasshopper via a file path panel
4. The plugin will connect to the model and return the predicted microclimate zone(s)

## 📦 For Plugin Users

Refer to the Grasshopper plugin’s documentation for setup instructions, including:
- Python requirements
- How to run the Flask server
- Example projects and testing data

## 🧠 Credits

Model and classification criteria developed as part of doctoral research on regenerative architecture by [Ana Zimbarg](https://github.com/yourusername).

---

Let me know if you'd like to add:
- DOI for a paper
- License file (MIT is standard)
- Badge for Zenodo, Hugging Face, or binder if you plan to host it elsewhere too
