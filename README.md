# LoomNet: Enhancing Multi-View Image Generation via Latent Space Weaving
![Teaser](https://github.com/GiulioFede/LoomNet/blob/main/github_files/teaser.png)

Generating consistent multi-view images from a single image remains challenging. Lack of spatial consistency often degrades 3D mesh quality in surface reconstruction. To address this, we propose LoomNet, a novel multi-view diffusion architecture that produces coherent images by applying the same diffusion model multiple times in parallel to collaboratively build and leverage a shared latent space for view consistency. Each viewpoint-specific inference generates an encoding representing its own hypothesis of the novel view from a given camera pose, which is projected onto three orthogonal planes. For each plane, encodings from all views are fused into a single aggregated plane. These aggregated planes are then processed to propagate information and interpolate missing regions, combining the hypotheses into a unified, coherent interpretation. The final latent space is then used to render consistent multi-view images. LoomNet generates 16 high-quality and coherent views in just 15 seconds. In our experiments, LoomNet outperforms state-of-the-art methods on both image quality and reconstruction metrics, also showing creativity by producing diverse, plausible novel views from the same input.

<table>
  <tr>
    <td>
      <a href="https://arxiv.org/pdf/2507.05499">
        <img src="https://github.com/GiulioFede/LoomNet/blob/main/github_files/arxiv_logo.jpg?raw=true" alt="arXiv" width="50"/>
      </a>
    </td>
    <td>
      <a href="https://arxiv.org/pdf/2507.05499">Read the paper on arXiv</a>
    </td>
  </tr>
</table>


<p float="left">
  <img src="[https://example.com/image1.png](https://github.com/GiulioFede/LoomNet/blob/main/github_files/risultati_multiview.png)" width="300" style="margin-right:10px"/>
  <img src="https://github.com/GiulioFede/LoomNet/blob/main/github_files/risultati_mesh.png" width="300"/>
</p>




