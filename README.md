# Few-Shot Domain Adaptation for Agricultural Crop-Weed Segmentation

This project explores the application of few-shot domain adaptation for crop-weed semantic segmentation in precision agriculture. It leverages deep learning techniques to adapt a model trained on a source domain (sugar beet crops) to new target domains (carrot and sunflower) with minimal labeled data.

## Key Features

- **DeepLabV3 with ResNet-50**: A robust architecture for semantic segmentation.
- **Few-Shot Learning**: Uses only 8-10 labeled images for target domain fine-tuning.
- **Data Augmentation**: Includes flipping, rotation, and color jittering to expand small datasets.
- **Domain Adaptation**: Demonstrates transfer learning to new crops while minimizing annotation costs.

## Dataset

- **Source Domain**: Sugar beet dataset with detailed pixel-wise annotations.
- **Target Domains**: Carrot and sunflower datasets, each with 8-10 labeled images for few-shot adaptation.

## Results

- Quantitative evaluation using pixel accuracy, F1 score, mean Intersection over Union (mIoU), and Mean Absolute Error (MAE).
- Qualitative results showing improved segmentation after few-shot adaptation.

## Challenges and Considerations

- Limited access to high-performance GPUs extended training and evaluation times.
- Small project team size (2 members) required balancing multiple tasks.
- Domain differences between crops presented adaptation challenges.

## Repository Structure

- `data/` : Dataset preparation scripts and sample images  
- `models/` : Model definitions and fine-tuning logic  
- `notebooks/` : Jupyter notebooks for experimentation  
- `results/` : Result figures and evaluation metrics  
- `utils/` : Utility functions (data loaders, metrics, etc.)  
- `main.py` : Main training and evaluation script

## How to Run

1. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
2. Prepare datasets (or download from provided links).
3. Run the main training script:
    ```bash
    python main.py --config config.yaml
    ```
4. View results in the `results/` directory.

## Additional Information

For detailed implementation and quantitative/qualitative results, please refer to the paper or the final report included in the `docs/` directory.

## License

This project is licensed under the MIT License.

---

**Contributors**:  
- Göktuğ Gökyılmaz (model implementation, data preparation, manuscript writing)  
- Berk Karaduman (visualization, result analysis, manuscript refinement)
