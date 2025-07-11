# LoomNet: Enhancing Multi-View Image Generation via Latent Space Weaving
:warning: The paper is under review and the code will be released soon.

## :blue_book:  <a href="https://arxiv.org/pdf/2507.05499" target="_blank">ArXiv Paper</a>

![Teaser](https://github.com/GiulioFede/LoomNet/blob/main/github_files/teaser.jpg)

### Abstract
Generating consistent multi-view images from a single image remains challenging. Lack of spatial consistency often degrades 3D mesh quality in surface reconstruction. To address this, we propose LoomNet, a novel multi-view diffusion architecture that produces coherent images by applying the same diffusion model multiple times in parallel to collaboratively build and leverage a shared latent space for view consistency. Each viewpoint-specific inference generates an encoding representing its own hypothesis of the novel view from a given camera pose, which is projected onto three orthogonal planes. For each plane, encodings from all views are fused into a single aggregated plane. These aggregated planes are then processed to propagate information and interpolate missing regions, combining the hypotheses into a unified, coherent interpretation. The final latent space is then used to render consistent multi-view images. LoomNet generates 16 high-quality and coherent views in just 15 seconds. In our experiments, LoomNet outperforms state-of-the-art methods on both image quality and reconstruction metrics, also showing creativity by producing diverse, plausible novel views from the same input.

### Some results on multi-view generation and mesh reconstruction
| ![Immagine 1](https://github.com/GiulioFede/LoomNet/blob/main/github_files/risultati_multiview.png) 
| ![Immagine 2](https://github.com/GiulioFede/LoomNet/blob/main/github_files/risultati_mesh.png) |


## :open_book: Citation

If you find this repository useful, please consider citing:

```
@misc{federico2025loomnetenhancingmultiviewimage,
      title={LoomNet: Enhancing Multi-View Image Generation via Latent Space Weaving}, 
      author={Giulio Federico and Fabio Carrara and Claudio Gennaro and Giuseppe Amato and Marco Di Benedetto},
      year={2025},
      eprint={2507.05499},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2507.05499}, 
}
```




