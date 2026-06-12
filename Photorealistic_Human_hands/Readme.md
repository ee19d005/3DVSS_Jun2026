## README




### Project Title: Photorealistic Hand Avatar Texturing with Palmar and Dorsal Hand Views
https://github.com/ee19d005/3DVSS_Jun2026/blob/main/Photorealistic_Human_hands/Photorealistic_Human_hands.ipynb
<img width="579" height="421" alt="UV texture" src="https://github.com/user-attachments/assets/de732f24-9a12-445e-97c9-913d2a6b49cf" />

Figure: Texture outputs given the Palmar and Dorsal Images of subjects

### Overview
This Colab notebook demonstrates a novel and efficient approach for generating photorealistic textures for 3D hand models. It specifically addresses the challenges of accurately representing both the palmar (front) and dorsal (back) sides of the hand by leveraging a ControlNet-based texture generation pipeline conditioned on anatomical priors.

The notebook covers:
-   **Environment Setup**: Installation of necessary libraries (`diffusers`, `ip-adapter`, `opencv-python`, `pyvista`, etc.) and downloading project assets- UV masks, UV normals, semantic masks,depth masks,and sample palmar and dorsal images.
-   **Input Preparation**: Loading and displaying control images (UV normal, depth, mask) and semantic UV maps, along with reference images for the back and palm of the hand.
-   **Semantic Masking**: Creating semantic masks for distinct hand regions (palm and back) to guide the diffusion process.
-   **Model Configuration**: Loading pre-trained ControlNet models (for normal and depth guidance) and configuring the IP-Adapter for style conditioning.
-   **Texture Generation**: Running the diffusion process separately for the back and palm of the hand, applying masks and specific prompts to generate region-specific textures.
-   **Texture Compositing**: Merging the generated back and palm textures based on semantic masks to create a final, cohesive UV albedo texture.
-   **Visualization**: Displaying the generated UV texture and applying it to a 3D hand mesh (`MANO_UV_right.obj`) for interactive visualization using `pyvista`.

This method enables rapid creation of personalized photorealistic hand avatars for various applications like XR, gaming, telepresence, and digital humans, generating high-quality UV texture maps in under one minute from minimal input.

### How to Run
1.  **Open in Google Colab**: Download the colab notebook and upload the `.ipynb` to your Google Drive, and open it with Google Colaboratory.
2.  **Run All Cells**: Navigate to `Runtime > Run all` in the Colab menu. This will execute all cells sequentially.
3.  **Execute Cells Individually**: Alternatively, you can run each cell one by one by clicking the "Play" button next to each code cell or by pressing `Shift + Enter`.
4.  **Interact with Visualizations**: After running the visualization cells, you can interact with the generated Plotly 3D figures (rotate, zoom, pan) and use the play/pause controls for animations.
