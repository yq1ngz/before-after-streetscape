# 🏛️ Before-After Streetscape Dataset

This dataset compiles and refines **400 before-and-after image pairs** of urban scenes and architectural transformations, sourced from the *New Traditional Architecture* initiative by [Michael Diamant (@michael_diamant)](https://x.com/michael_diamant) on X. The images have been processed to remove watermarks and visual obstructions (such as trees), making them suitable for **academic research**, **visual perception studies**, and **machine learning tasks**.



## 📁 Dataset Structure
```text
BeforeAfterStreetscape/
├── 1_Original images/ # Screenshots from original tweets
├── 2_Separate images without watermark/ # Cropped and cleaned 'before/after' images
├── 3_Images without trees/ # Tree-removed images for clear façade analysis
└── 4_3M VAS results/ # Visual attention predictions via 3M VAS
```


## 🖼️ Image Processing Notes

- **Watermark Removal**: Image inpainting techniques were used to remove text overlays or watermarks.
- **Tree/Object Removal**: Manual + AI segmentation was used to eliminate trees and obstructions in front of buildings, highlighting the transformation clearly.
- **Visual Attention Simulation**: We applied 3M’s Visual Attention Software (VAS) to simulate eye fixation heatmaps on each image.
- **Image Alignment**: Each image pair was normalized to consistent resolution and central framing.


## 📊 Potential Applications

- Studies on aesthetic preference between traditional and modern architecture  
- Visual impact analysis of urban or architectural renovation  
- Training data for generative or comparative models in architecture and planning  
- Educational material in urban design, landscape architecture, and planning


## 📎 Source & Copyright

All original images were publicly posted by [@michael_diamant](https://x.com/michael_diamant) on the X platform.  
This dataset is intended for **non-commercial academic and research purposes only**.  
For commercial use or redistribution, please contact the original author for permission.



## 🔧 Future Plans

- [ ] Add metadata for each image pair (e.g., city, country, building style)  
- [ ] Provide code for automatic image alignment and formatting  
- [ ] Release a version on Hugging Face Datasets  
- [ ] Add baseline models for visual impact scoring and style transfer  
