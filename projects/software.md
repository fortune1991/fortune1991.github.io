---
layout: default
title: Software
permalink: /projects/software/
---

# Software

During my year of travelling, I’ve been developing a range of side projects to expand my skill set. Each project explores different technologies and libraries in the Python ecosystem.

## ICU_Grow
<p align="center">
  <img src="/assets/img/icu_grow.jpg" alt="ICU_Grow_image" width="850">
</p>

**Technologies:** Micropython, AWS, Async, Ntfy, Open API's, Raspberry Pi Pico

**Description:** ICU_Grow is an IoT enabled, automated greenhouse for my garden.

**Key Features:**
- Temperature, Humidity, Light and Plant Moisture Sensors
- LCD Screen to display data to users. Includes current condition plus 24hr average, high and low readings
- Data logs stored on microSD card
- Actuated roof ventilators, heating mats and cooling fans to control environmental conditions
- Irrigation feedback
- Cloud data pipeline to store logs, visualise data and analyse long term trends of environmental conditions
- Phone notifications and alerts for extreme conditions

**GitHub:** [Link to repository](https://www.github.com/fortune1991)

**Demonstration Video:**

<p align="center">
  <div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/AugEfShF2M0"
      title="ICU Grow Demo"
      frameborder="0"
      allowfullscreen>
    </iframe>
  </div>
</p>

<style>
.video-container {
  position: relative;
  width: 100%;
  max-width: 850px; /* optional max width */
  aspect-ratio: 16 / 9;
  margin: 0 auto;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>

## MoneyPots

**Demo Version:**  [Link to app](https://moneypots-beta.streamlit.app/)

<p align="center">
  <img src="/assets/img/moneypots.jpg" alt="moneypots_image" width="850">
</p>

**Technologies:** Python, MySQL, AWS, Grafana, Streamlit

**Description:** Money Pots is a budgeting calculator built for travelers. It enables users to divide their savings into Vaults and Pots, helping them manage funds across different parts of a trip. A built-in budget forecasting tool estimates what your balance _should_ be at any given point to stay on track. The project has been developed iteratively, allowing me to explore the impact of new features and architectural changes within an evolving codebase.

**Key Features:**
- Persistent data storage with MySQL hosted on AWS
- UI created using Streamlit
- Budget forcasting tool, with visualisations created using Grafana

**Build Diary:** [Click here!](/projects/build_diaries/moneypots)

**GitHub:** [Link to repository](https://github.com/fortune1991/money_features)



