# Dynamic Playlists Vimeo Gallery

This project enhances Vimeo video delivery by creating a dynamic playlist gallery where users can:

* Select **any criteria** (e.g., topic, keyword, etc) to view relevant live events and videos.
* Immediately engage with a featured video upon page load.
* Browse and choose from related videos in a thumbnail grid.
* Seamlessly switch between videos by clicking thumbnails.
* Easily return to the featured video after exploring other content.


## Features

* **Criteria Selection:** Dynamically loads the featured video and related videos based on the chosen criteria. See Figure 1 for a diagram of a multi-language criteria selection UI.
* **Featured Video:** Prominently displays the currently playing video.
* **Thumbnail Grid:** Showcases related videos for easy browsing.
* **Featured Video Thumbnail:** A dedicated thumbnail for quick access to the initially selected video.

<img width="256" align="center" src="https://github.com/user-attachments/assets/81d358d3-cba5-4f0c-8293-56dbc60a5122">

<p align="left">Figure 1. Diagram of a multi-language criteria selection UI.</p>

## Technical Implementation

This prototype leverages the Vimeo API to overcome limitations of Vimeo Showcases, such as the restriction of one event per showcase and the lack of API methods for dynamic content updates. See Figure 2 for a diagram of the implementation logic workflow.

## UML Workflow

![image](https://github.com/user-attachments/assets/26651cb2-38b2-4d3a-8ee9-0c372488a945)
<p align="left">Figure 2. UML Sequence Diagram .</p>

**Key aspects:**

* **`changeFeaturedVideo()` function:** Fetches and updates the featured video and video grid based on the selected criteria.
* **`handleThumbnailClick()` function:** Manages video switching and thumbnail grid updates.
* **Dynamic Thumbnail Generation:**  Thumbnails are generated dynamically based on the chosen criteria (e.g., tags, keywords, etc.).

## Getting Started

1. **Clone the repository:** `git clone https://github.com/your-username/Dynamic-Playlists-for-Vimeo.git`
2. **Replace `{TOKEN}`:** In the `index.html` file, replace `{TOKEN}` with your actual Vimeo API access token. 
3. **Update Criteria and Video IDs:** Modify the `index.html` to include your desired criteria (e.g., dropdown with topics, a search bar) and corresponding video IDs.
4. **Open `index.html`:** Open the file in your web browser.
