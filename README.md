# A dynamic playlist gallery for Vimeo videos

This project enhances Vimeo video delivery by creating a dynamic playlist gallery where users can:

* Select any criteria (e.g., topic, keyword, etc) to view relevant live events and videos.
* Immediately engage with a featured video upon page load.
* Browse and choose from related videos in a thumbnail grid.
* Seamlessly switch between videos by clicking thumbnails.
* Easily return to the featured video after exploring other content.

The following short video shows the solution in action:

https://github.com/user-attachments/assets/98cb2a50-81a4-43a3-b0fb-6f7f5d4746a6

## Features

The dynamic playlist gallery offers the following features.

* **Criteria Selection:** The gallery dynamically loads the featured video and related videos based on the chosen criteria. See Figure 1 for a wireframe of the UI. 

<img width="256" align="center" src="https://github.com/user-attachments/assets/81d358d3-cba5-4f0c-8293-56dbc60a5122">
<p align="left">Figure 1. Wireframe of a multi-language criteria selection UI.
</p>

* **Featured Video:** The gallery prominently displays the initially selected video on load and switches videos dynamically as the user requests them.
* **Thumbnail Grid:** The thumbnail grid showcases related videos for easy browsing. The thumbnail images are dynamically generated. A dedicated thumbnail image representing the original featured video enables the user to return to it quickly.
  
Key aspects of the workflow are as follows:


* **The `changeFeaturedVideo()` function.** This fetches and updates the featured video and video grid based on the selected criteria.
* **The `handleThumbnailClick()` function.** This manages video switching and thumbnail grid updates.
* **Dynamic Thumbnail Generation.** As mentioned previously, thumbnails are generated dynamically based on the chosen criteria.

See Figure 2 for a diagram of the implementation logic workflow.

![image](https://github.com/user-attachments/assets/26651cb2-38b2-4d3a-8ee9-0c372488a945)
<p align="left">Figure 2. UML Sequence Diagram .</p>

## How to use this repo

To get started with the gallery in your own projects:

1. **Clone the repository** by running the following: `git clone https://github.com/your-username/Dynamic-Playlists-for-Vimeo.git`
2. **Replace the `{TOKEN}`** placeholder in the index.html file with your Vimeo API access token. For more information, see [Working with Authentication](https://developer.vimeo.com/api/authentication) on the Vimeo developer site.
3. **Modify `index.html`** according to the way that you want to populate the thumbnail grid, maybe with a dropdown menu of preselected criteria for the user to choose from or even a search bar implementation. Make sure to capture the video IDs of the corresponding videos.
4. **Open `index.html`** in your web browser.

