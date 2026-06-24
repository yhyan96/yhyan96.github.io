---
layout: homepage
---

## About Me

I am currently a Lecturer at Shanghai Maritime University, and I obtained my Ph.D. in June 2025 from the School of Information Science and Technology, ShanghaiTech University. My research interests lie at the intersection of Security and Privacy Protection and Human-Computer Interaction, with a particular focus on privacy-enhancing technologies for real-world and emerging sensing systems (e.g., biometric authentication systems and wireless sensing systems). 

<!-- ## Research Interests

- **Computer Vision:** image recognition, image generation, video captioning
- **Machine Learning:** meta-learning, incremental learning, transfer learning -->

## News
<!-- Good news: &#128512;  -->
<!-- Bad news: &#128546; -->

<div id="news-section">
  <ul id="news-list" style="padding-left: 0; margin-top: 0; margin-bottom: -15px">
    <li><strong>[Mar. 2026]</strong> 😊 Our paper about LoRa-to-mobile bridging is accepted to SECON 2026.</li>
    <li><strong>[Aug. 2025]</strong> 😊 Our paper about in-model spy is accepted to RAID 2025.</li>
    <li><strong>[Aug. 2025]</strong> 😊 I have joined SHMTU.</li>
    <li><strong>[Jun. 2025]</strong> 😊 I completed my CS PhD from ShanghaiTech.</li>
    <li><strong>[Mar. 2025]</strong> 😊 Our demo about 2FA for Fingerprint will be demonstrated in Sensys 2025.</li>
    <li><strong>[Jan. 2025]</strong> 😊 Our paper about 2FA for Fingerprint is accepted to USENIX Security 2025.</li>
    <li><strong>[Oct. 2024]</strong> 😊 Our paper about Privacy Protection in Wi-Fi Sensing is accepted to ACSAC 2024.</li>
    <li><strong>[May. 2024]</strong> 😊 Our paper about Privacy-enhanced Fingerprint Enrollment is accepted to CCS 2024.</li>
    <li><strong>[Feb. 2023]</strong> 😊 Our paper is accepted to PMC Vol.90.</li>
    <li><strong>[Feb. 2022]</strong> 😊 Our paper is accepted to CHI 2022.</li>
    <li><strong>[Feb. 2022]</strong> 😊 Our paper is accepted to USENIX Security 2022.</li>
    <li><strong>[Aug. 2021]</strong> 😊 Our paper is accepted to GLOBECOM 2021.</li>
    <li><strong>[Jan. 2021]</strong> 😊 Our demo will be demonstrated in PerCom 2021.</li>
    <li><strong>[Dec. 2020]</strong> 😊 Our paper is accepted to PerCom 2021.</li>
  </ul>

  <button id="news-toggle" style="border:none;background:none;color:#002D72;cursor:pointer;font-weight:bold;padding:0;">
    More
  </button>
</div>


{% include_relative _includes/publications.md %}

<!-- {% include_relative _includes/services.md %} -->

<script>
document.addEventListener('DOMContentLoaded', function () {
  const items = Array.from(document.querySelectorAll('#news-list li'));
  const visibleCount = 5;
  const toggle = document.getElementById('news-toggle');
  if (!toggle || items.length <= visibleCount) return;

  let expanded = false;
  function update() {
    items.forEach((item, index) => {
      item.style.display = index < visibleCount || expanded ? '' : 'none';
    });
    toggle.textContent = expanded ? 'Less' : 'More';
  }

  expanded = false;
  update();

  toggle.addEventListener('click', function () {
    expanded = !expanded;
    update();
  });
});
</script>