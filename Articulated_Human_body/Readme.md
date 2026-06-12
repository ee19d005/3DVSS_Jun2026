## README




### Project Title: SMPLX Model Visualization and Animation
https://github.com/Meghnashankr23/3DVSS_June2026/blob/main/SMPLX_Animate.ipynb
<img width="1013" height="565" alt="image" src="https://github.com/user-attachments/assets/d12ca9df-1112-444f-b2a9-7a909df2b529" />
Image Source: https://github.com/facebookresearch/frankmocap/issues/91
### Overview
This Colab notebook demonstrates the loading, manipulation, visualization, and animation of the SMPLX human body model. It uses Python libraries such as `smplx` for model functionality, `trimesh` for 3D mesh processing, and `plotly` for interactive 3D visualizations and animations.

The notebook covers:
-   **Environment Setup**: Installation of necessary libraries (`smplx`, `trimesh`, `gdown`, `plotly`, `imageio`).
-   **Model Loading**: Downloading and initializing the SMPLX model files.
-   **Model Inspection**: Verifying model output dimensions (vertices and joints).
-   **Body Manipulation**: Adjusting body shape (`betas`) and pose (`body_pose`) parameters.
-   **Visualization**: Static and interactive 3D rendering of the SMPLX mesh and its joints using `trimesh` and `plotly`.
-   **Animation**: Creating dynamic animations of pose variations and custom pose sequences.



### How to Run
1.  **Open in Google Colab**: Download the colab notebook and upload the .ipynb to your Google Drive, and open it with Google Colaboratory.
2.  **Run All Cells**: Navigate to `Runtime > Run all` in the Colab menu. This will execute all cells sequentially.
3.  **Execute Cells Individually**: Alternatively, you can run each cell one by one by clicking the "Play" button next to each code cell or by pressing `Shift + Enter`.
4.  **Interact with Visualizations**: After running the visualization cells, you can interact with the generated Plotly 3D figures (rotate, zoom, pan) and use the play/pause controls for animations.

