---
layout: default
title: "Adopt a Dog"
permalink: /dogs
---

<h1 style="text-align:center; margin-top: 2rem;">Adopt a Dog</h1>

<!-- Dog Grid -->
<div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 1.5rem; padding: 2rem;">

  <!-- Example Dog -->
  <div style="text-align: center;">
    <img src="{{ '/assets/dogs/dog1.png' | relative_url }}" 
         alt="Buddy — Playful and friendly" 
         style="width:100%; border-radius:12px; cursor:pointer; transition: transform 0.3s ease;"
         onclick="openModal(this)">
    <p style="margin-top: 0.5rem; font-weight:600;">Buddy</p>
    <p>Playful and friendly</p>
  </div>

  <div style="text-align: center;">
    <img src="{{ '/assets/dogs/dog2.png' | relative_url }}" 
         alt="Luna — Shy but sweet" 
         style="width:100%; border-radius:12px; cursor:pointer; transition: transform 0.3s ease;"
         onclick="openModal(this)">
    <p style="margin-top: 0.5rem; font-weight:600;">Luna</p>
    <p>Shy but sweet</p>
  </div>

  <div style="text-align: center;">
    <img src="{{ '/assets/dogs/dog3.png' | relative_url }}" 
         alt="Rex — Senior gentleman" 
         style="width:100%; border-radius:12px; cursor:pointer; transition: transform 0.3s ease;"
         onclick="openModal(this)">
    <p style="margin-top: 0.5rem; font-weight:600;">Rex</p>
    <p>Senior gentleman</p>
  </div>

  <div style="text-align: center;">
    <img src="{{ '/assets/dogs/dog4.png' | relative_url }}" 
         alt="Bella — Full of energy" 
         style="width:100%; border-radius:12px; cursor:pointer; transition: transform 0.3s ease;"
         onclick="openModal(this)">
    <p style="margin-top: 0.5rem; font-weight:600;">Bella</p>
    <p>Full of energy</p>
  </div>

  <!-- Add more dogs here following the same pattern -->

</div>

<!-- Popup Modal -->
<div id="modal" 
     style="display:none; position:fixed; top:0; left:0; width:100%; height:100%; 
            background:rgba(0,0,0,0.8); justify-content:center; align-items:center; flex-direction:column; z-index:1000;">
  <img id="modal-img" src="" 
       style="max-width:90%; max-height:80%; border-radius:10px; box-shadow:0 0 20px rgba(255,255,255,0.3);">
  <p id="modal-caption" 
     style="color:white; margin-top:1rem; font-size:1.2rem; text-align:center;"></p>
</div>

<script>
function openModal(img) {
  const modal = document.getElementById('modal');
  const modalImg = document.getElementById('modal-img');
  const caption = document.getElementById('modal-caption');

  modalImg.src = img.src;
  caption.textContent = img.alt;
  modal.style.display = 'flex';

  modal.onclick = () => {
    modal.style.display = 'none';
  };
}
</script>
