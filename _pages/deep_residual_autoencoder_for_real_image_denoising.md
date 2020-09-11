---
title: "Deep Residual Autoencoder for Real Image Denoising"
permalink: /deep_residual_autoencoder_for_real_image_denoising
author_profile: false
---

<script src="assets/js/plugins/BeerSlider.js"></script>
<script src="assets/js/plugins/select.js"></script>

## Abstract

Image denoising is one of the fundamental problems in low-level computer vision since it has found more and more real-world applications every day. Various approaches have been used for image denoising throughout the years such as block-matching and 3D filtering (BM3D). In the recent years learning-based approaches have outperformed the traditional methods such as BM3D. However, most of these learning-based methods makes the assumption that the real-world noise is fully modeled with various noise model such as additive white Gaussian noise (AWGN). These methods struggle to achieve outstanding performance when it comes to real-world noide. With the recent release of real-world noise datasets such as Smartphone Image Denoising Dataset (SIDD) and Darmstadt Noise Dataset (DND), the limitation caused by lack of real world noise data has eliminated. In this paper, we propose a deep convolutional autoencoder network combined with symmetric residual connections for real image denoising. We used the real-world images provided by SIDD for the training of the proposed model. Also, we have experimented with L1, L2, SSIM, MS-SSIM and sum of L1 and MS-SSIM loss functions in order to optimize the performance of our proposed model both qualitatively and quantitative. Our experimental results show that our proposed model outperforms the traditional methods and offers similar performance with state-of-the-art methods in blind real image denoising.

---

<div class="paper-info">

  <div class="paper-info paper-image">
    <img src="assets/images/cs402_report_image.png" href="./assets/cs402_report.pdf">
  </div>

  <div class="paper-info paper-data">

  <ul>
    <li><b>Paper</b></li>
    <li>Doğa Yılmaz "Deep Residual Autoencoder for Real Image Denoising".</li>
    <li>Supervised by Assist. Prof. Dr. M. Furkan Kıraç.</li>
    <li><b>Paper: </b><a href="./assets/deep_residual_autoencoder_for_real_image_denoising.pdf">PDF Link</a></li>
    <li><b>Code: </b> <a href='https://github.com/yilmazdoga/Deep_Residual_Autoencoder_for_Real_Image_Denoising'>PyTorch Implementation</a></li>
  </ul>

  </div>

</div>


## Results

<select id="input" onchange="selector()" name="dropdown">
   <option value="compare0">Example 1: Noisy vs Ground-Truth</option>
   <option value="compare1">Example 1: Noisy vs Denoised</option>
   <option value="compare2">Example 1: Denoised vs Ground-Truth</option>
   <option value="compare3">Example 2: Noisy vs Ground-Truth</option>
   <option value="compare4">Example 2: Noisy vs Denoised</option>
   <option value="compare5">Example 2: Denoised vs Ground-Truth</option>
   <option value="compare6">Example 3: Noisy vs Ground-Truth</option>
   <option value="compare7">Example 3: Noisy vs Denoised</option>
   <option value="compare8">Example 3: Denoised vs Ground-Truth</option>
</select>

<div id="compare0" class="beer-container">
  <header>

  </header>
  <div id="slider0" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_0.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_0.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare1" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider1" class="beer-slider" data-beer-label="Denoised">
    <img src="assets/images/DRA_Examples/DENOISED_0.png"  alt="Denoised">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_0.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare2" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider2" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_0.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Denoised">
      <img src="assets/images/DRA_Examples/DENOISED_0.png"  alt="Denoised">
  </div>
</div>
</div>

<div id="compare3" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider3" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_1.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_1.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare4" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider4" class="beer-slider" data-beer-label="Denoised">
    <img src="assets/images/DRA_Examples/DENOISED_1.png"  alt="Denoised">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_1.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare5" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider5" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_1.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Denoised">
      <img src="assets/images/DRA_Examples/DENOISED_1.png"  alt="Denoised">
  </div>
</div>
</div>

<div id="compare6" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider6" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_2.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_2.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare7" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider7" class="beer-slider" data-beer-label="Denoised">
    <img src="assets/images/DRA_Examples/DENOISED_2.png"  alt="Denoised">
    <div class="beer-reveal" data-beer-label="Noisy">
      <img src="assets/images/DRA_Examples/NOISY_2.png"  alt="Noisy">
  </div>
</div>
</div>

<div id="compare8" style = "display: none;" class="beer-container">
  <header>

  </header>
  <div id="slider8" class="beer-slider" data-beer-label="Ground-Truth">
    <img src="assets/images/DRA_Examples/GT_2.png"  alt="Ground-Truth">
    <div class="beer-reveal" data-beer-label="Denoised">
      <img src="assets/images/DRA_Examples/DENOISED_2.png"  alt="Denoised">
  </div>
</div>
</div>


<script>
  new BeerSlider( document.getElementById( "slider0" ) );
  new BeerSlider( document.getElementById( "slider1" ) );
  new BeerSlider( document.getElementById( "slider2" ) );
  new BeerSlider( document.getElementById( "slider3" ) );
  new BeerSlider( document.getElementById( "slider4" ) );
  new BeerSlider( document.getElementById( "slider5" ) );
  new BeerSlider( document.getElementById( "slider6" ) );
  new BeerSlider( document.getElementById( "slider7" ) );
  new BeerSlider( document.getElementById( "slider8" ) );
</script>