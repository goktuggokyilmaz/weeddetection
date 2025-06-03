# Few-Shot Domain Adaptation for Agricultural Crop-Weed Segmentation

This project explores **few-shot domain adaptation** for crop-weed semantic segmentation in precision agriculture. Leveraging **DeepLabV3 with a ResNet-50 backbone**, the project demonstrates how to adapt a model trained on a source domain (sugar beet crops) to new target domains (carrot and sunflower) using only 8–10 labeled images per target domain.

---

## Key Highlights

- **DeepLabV3 with ResNet-50**: A proven architecture for semantic segmentation tasks.
- **Few-Shot Learning**: Uses minimal labeled data for target domain fine-tuning.
- **Data Augmentation**: Includes flips, rotations, and color jittering to make the most of limited data.
- **Domain Adaptation**: Validates that even with very few labeled samples, significant performance gains can be achieved.

---

## Project Structure

- **WeedDetectionProject.ipynb**: The single Jupyter notebook containing the full implementation, including:
  - Data loading and preprocessing
  - Model setup and few-shot adaptation pipeline
  - Evaluation metrics and visualization of segmentation outputs

- **Datasets**: Three separate dataset folders (not provided in this repository) referenced and described in the project report:
  - Sugar beet (source domain)
  - Carrot (target domain)
  - Sunflower (target domain)

For dataset sources and preparation details, please see the references section of the accompanying project report (`WeedDetectionProject.pdf`).

---

## Running the Project

1. Clone the repository and open the Jupyter notebook:
    ```bash
    jupyter notebook WeedDetectionProject.ipynb
    ```

2. Follow the notebook’s cells to run data preparation, model training, and evaluation.

---

## Results

The project includes:
- **Quantitative results**: Pixel accuracy, F1 score, mean Intersection over Union (mIoU), and Mean Absolute Error (MAE).
- **Qualitative results**: Visualizations of segmentation performance before and after few-shot adaptation.

For a detailed presentation of results and methodology, see the final report:  
📄 **`WeedDetectionProject.pdf`**

---

## Notes and Considerations

- **Hardware**: Limited GPU access extended training times compared to typical deep learning projects.
- **Small team (2 members)**: Balanced data handling, model implementation, and report writing.
- **Domain gap**: The effectiveness of adaptation depends on morphological similarities between crops.

---

## License

This project is licensed under the MIT License.

---

**Contributors**:  
- Göktuğ Gökyılmaz (model implementation, data preparation, manuscript writing)  
- Berk Karaduman (visualization, result analysis, manuscript refinement)

