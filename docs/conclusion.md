## Create the Skill-Based Queue

<video src="https://raw.githubusercontent.com/WebexCC-SA/LAB-2310/main/docs/assets/VD1.mp4" width="500" controls> </video>

<video style="width: 100%; max-width: 800px; height: auto;" controls preload="metadata">
  <source src="https://raw.githubusercontent.com/WebexCC-SA/LAB-2310/main/docs/assets/VD1.mp4" type="video/mp4">
</video>

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


