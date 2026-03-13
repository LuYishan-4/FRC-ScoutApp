# FRC Scouting System - 7632

<img src="https://github.com/team7632/FRC-ScoutApp/blob/master/assets/images/favicon.png" width="100">

![Node.js](https://img.shields.io/badge/Node.js-v16%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-4.x-000000?style=for-the-badge&logo=express&logoColor=white)
![NAS](https://img.shields.io/badge/NAS-Hosted-blue?style=for-the-badge&logo=synology&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## Table of Contents
* [System Overview](#system-overview)
* [Quick Start](#quick-start)
  * [Login](#login)
  * [Creating & Joining Rooms](#creating--joining-rooms)
  * [Match Scouting](#match-scouting)
* [Pit Scouting](#pit-scouting)

---

## System Overview

Welcome to **FRC Scouting System - 7632**! This is a data collection and management system designed specifically for FIRST Robotics Competition (FRC). This manual will guide you through everything from data synchronization to on-site sampling.

---

## Quick Start

### Login
Before scouting, please log in using your **Google Account**.

---

## Creating & Joining Rooms

<img src="https://github.com/team7632/FRC-ScoutApp/blob/master/screenshot/Screenshot_20260216_234657.jpg" width="400">

On the home page, you will see three buttons:
* **Create New Room**
* **Join Server Room**
* **Fetch TBA Schedule**

### Create New Room
* Allows users to create a custom room with specific team numbers and matches.
* Enter a **ROOM IDENTIFIER** and click **LAUNCH DATA HUB**.
* The host can manage team assignments by clicking the shield icon in the top right.

### Join Server Room
* Join an existing room created by a host to start scouting assigned teams.

<div align="center">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234709.jpg" width="350">
<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234800.jpg" width="350">
</div>

### Fetch TBA Schedule
For automated task distribution:
* Search for the year and event (e.g., 2025, New Taipei City).
* If successful, the system displays **TBA PAYLOAD READ** and preloads all qualification match data.
* Click **LAUNCH DATA HUB** to create the room.

---

## Match Scouting

### Preparation
* After joining a room, wait for the host to assign a team.
* When the screen shows a team color and number, click **START SCOUTING**, verify the match info, and click **READY**.

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_234750.jpg" width="400">

---

### Autonomous (AUTO) Phase

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235008.jpg" width="400">

* Use "**+**" and "**-**" to record scores.
* Toggles available for **Leave Line** and **Auto Hang**.
* **Path Drawing**: Tap the map to create a path, use **Command** for actions, and **Play** to review.

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235014.jpg" width="400">

---

### Teleoperated & Endgame
* Record scores as in the AUTO phase.
* In the **ENDGAME STATUS** section, select the robot's hanging level (or "NONE").
* Click **COMPLETE & SYNC DATA** once the match ends.

---

### Post-Match Analysis

<img src="https://raw.githubusercontent.com/team7632/FRC-ScoutApp/master/screenshot/Screenshot_20260216_235030.jpg" width="400">

* **Shooting Accuracy**: Slider from "Low Precision" to "Sniper Accuracy."
* **Driver Performance**: Quick tags for evaluation.
* **Scout Notes**: Free-text for stability, defense, or mechanical issues.
* Click **FINISH MATCH ANALYSIS** to upload to the cloud.

---

## Pit Scouting

Access **Pit Mode** via the four-square icon on the home screen.

1.  **Pit Tracker**: Overview of scouting progress and team list.
2.  **Photo**: Capture or upload robot images for visual identification.
3.  **Spec**: Record hardware like **Drivetrain Type** and **Max Capacity**.
4.  **Path**: Map out the team's intended autonomous routines with `Point`, `Wait`, and `Command` tools.

> **Sync**: Click **UPLOAD PIT DATA** to save the technical profile to the database.
