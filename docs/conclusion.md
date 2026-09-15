## Create the Skill-Based Queue

<details>
<summary><b>🎥 Video Walkthrough: Create Skill-Based Queue</b></summary>
<br>
<video style="width: 100%; max-width: 800px; height: auto;" controls controlsList="nodownload" preload="metadata">
  <source src="https://raw.githubusercontent.com/WebexCC-SA/LAB-2310/main/docs/assets/VD1.mp4" type="video/mp4">
</video>
</details>

<style>
  .doc-animation {
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    max-width: 100%;
    display: block;
    margin: 10px 0;
  }
</style>

<!-- 2. The HTML: Calls the class to apply those styles -->
<video class="doc-animation" autoplay loop muted playsinline>
  <source src="https://raw.githubusercontent.com/WebexCC-SA/LAB-2310/main/docs/assets/VD1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<!-- Embedded CSS Styling -->
<style>
  .doc-video-card {
    max-width: 800px;
    margin: 1.5rem auto;
    border: 1px solid #d0d7de;
    border-radius: 8px;
    overflow: hidden;
    background-color: #f6f8fa;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  }

  .doc-video-wrapper {
    position: relative;
    width: 100%;
    background-color: #000000;
  }

  .doc-video-wrapper video {
    display: block;
    width: 100%;
    height: auto;
    border: none;
  }

  .doc-video-caption {
    padding: 10px 16px;
    font-size: 0.85rem;
    color: #57606a;
    background-color: #ffffff;
    border-top: 1px solid #d0d7de;
  }
</style>

<!-- Video Component HTML -->
<div class="doc-video-card">
  <div class="doc-video-wrapper">
    <video 
      controls 
      autoplay 
      loop 
      muted 
      playsinline 
      preload="metadata">
      <!-- Replace the src URL below with your actual MP4 file path or GitHub URL -->
      <source src="https://raw.githubusercontent.com/WebexCC-SA/LAB-2310/main/docs/assets/VD1.mp4" type="video/mp4" />
      Your browser does not support the video tag.
    </video>
  </div>
  <div class="doc-video-caption">
    <strong>Demo:</strong> Walkthrough demonstration of the feature setup.
  </div>
</div>



> 💡 **Tip:** Click the **`⋮`** on the video player and select **Picture-in-Picture** to keep the video floating on screen while performing lab steps in Control Hub.

1. In the **Contact Center** navigation pane, select **Queues** under the **Customer Experience** section.

2. Click the **Create Queue** button.

3. Configure the general queue settings using the table below:

| Field Name | Value / Setting | Description |
| --- | --- | --- |
| **Queue Name** | `WebexOne_SBR_Queue_[name]`
| **Contact Direction** | **Inbound Queue** | 
| **Channel Type** | **Telephony** | 

4. Scroll to **Contact Routing Settings**, enable **Skill-Based Routing**, and configure the following:
	* **Skill Assignment Type:** Select **Assign skills in flows**.
	* **Agent Assignment:** Select **Teams**.
	* **Routing Pattern:** Select **Longest Available**.

5. Under **Call Distribution**, create a new group and add your designated team: `WebexOne_Team_[num]`.

6. Scroll to **Advanced Settings** and verify the following parameters:
	* **Service Level Threshold:** `30` seconds
	* **Maximum Time in Queue:** `30` seconds
	* **Default Music in Queue:** `defaultmusic_on_hold.wav`


7. Click **Save** to finalize and create the queue.


