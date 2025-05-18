[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/warframe-tools/Task-Checklist) ![HTML5 Badge](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=fff&style=flat) ![CSS3 Badge](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=fff&style=flat) ![JavaScript Badge](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=000&style=flat) 

# Warframe Task Checklist Web App

A simple, client-side web application to help Warframe players track their daily, weekly, and bi-weekly in-game tasks.

## Repository Updates

This repository will be updated (if changes are made) on the weekly reset (00:00 UTC) to avoid resets to the application hosted on Pages. To avoid any accidental resets of your progress, please fork this repository and host it yourself, or download it and use it locally (and make sure to update it weekly with any changes if needed).

## Description

This tool provides checklists for common recurring activities in Warframe. It saves your progress directly in your browser's local storage, automatically resets daily and weekly tasks based on UTC time, and offers a few customization options.

## Fan Made Reviews/Showcase

[![Conquering Productions](https://img.youtube.com/vi/fHOz21Zj0Yc/mqdefault.jpg)](https://www.youtube.com/watch?v=fHOz21Zj0Yc)
**Conquering Productions**

## Features

* **Comprehensive Task Lists:** Includes common Daily, Weekly, and a new "Other Tasks" section.
    * **Collapsible Sections:** Each major section can be expanded or collapsed for a cleaner view.
    * **Subtasks:** Daily World Syndicate tasks are broken down into collapsible subtasks with linked parent/child checking behavior.
* **Task Visibility Control:**
    * **Hide Individual Tasks:** Each task has an eye icon (👁️) to hide it from view. Hidden tasks are saved and persist across sessions.
    * **Hide Entire Sections:** If all tasks within a section are individually hidden, a "Hide Section" button will appear on the section header, allowing you to manually hide the entire section. This state is also saved.
* **Local Progress Saving:** Your checked tasks, hidden task preferences, and notification settings are saved directly in your browser's local storage.
    * **Version-Aware Storage:** Save data now persists across minor and patch updates (e.g., v2.0.x, v2.1.x, v2.2.x). A new save file is only created on major version changes (e.g., v2.x.x to v3.0.0).
* **Dynamic Timers & Resets:**
    * **Automatic Daily/Weekly Resets:**
        * Daily tasks reset automatically after 00:00 UTC.
        * Weekly tasks reset automatically after Monday 00:00 UTC.
        * Section headers display a dynamic countdown timer (e.g., "Resets in HH:MM:SS") for these.
    * **Baro Ki'Teer Tracker (in "Other Tasks"):**
        * Displays a live countdown to Baro's arrival ("Arrives in Xd HH:MM:SS").
        * Switches to a departure countdown ("Leaves in HH:MM:SS") when he is present.
    * **8-Hour Rotating Vendor Tasks (in "Other Tasks"):**
        * Includes tasks for Grandmother, Archimedean Yonta, and Loid (Necralisk).
        * These tasks reset every 8 hours (00:00, 08:00, 16:00 UTC).
        * Each has an individual countdown timer showing time until its next reset.
* **Optional Browser Notifications (for "Other Tasks"):**
    * Each task in the "Other Tasks" section (Baro, Grandmother, Yonta, Loid) has a Bell icon (🔔).
    * Click the Bell icon to opt-in to receive browser notifications for that specific task.
        * **Baro Ki'Teer:** Get notified when he arrives and shortly before he departs.
        * **8-Hour Vendors:** Get notified when their stock resets.
    * Notifications are visual popups only (no sound).
    * Notification preferences are saved locally. The icon turns green when active.
* **Modal Options Menu:**
    * A hamburger icon (☰) on the top right opens a modal menu.
    * **Manual Reset Options:** Buttons to manually reset "Daily Checks," "Weekly Checks," or "All Checks" (with two-click confirmation).
    * **Unhide All Tasks:** A button to unhide all individually hidden tasks and manually hidden sections (with confirmation).
* **Customizable Theme:**
    * Toggle between a dark mode (default) and a light mode.
    * Theme preference is saved locally.
* **Dynamic Background:**
    * Features a daily rotating background image.
* **User-Friendly Error Handling:**
    * Displays clear error messages if issues occur (e.g., problems saving to local storage).
    * Includes a "Copy" button in the error display for easy reporting.
* **Responsive Design:** Styled with Tailwind CSS for a generally responsive layout.
* **Footer Information:** Includes links to relevant resources (WarframeTools, GitHub, License, Warframe Hub, Warframe Wiki, FrameHub), app version, and current Warframe version.

## How to Use

There are a few ways to use the Warframe Task Checklist:

1.  **Directly from Github Pages on this repository (Recommended for most users):**
    * Go directly to the Github Page that is run from this repository! https://warframetools.com/Task-Checklist/

2.  **GitHub Pages:**
    * The easiest way is to **fork this repository** to your own GitHub account.
    * Enable GitHub Pages for your forked repository (usually under `Settings > Pages`, select the `main` branch and `/ (root)` folder).
    * You will then have your own live version of the checklist that you control.
    * **Update Schedule:** The main `warframe-tools/Task-Checklist` repository will aim to be updated with new tasks or game version changes around the weekly reset (Monday 00:00 UTC) to avoid disrupting users mid-week. You can then pull these updates into your fork.

3.  **Download and Run Locally:**
    * Download the source package below and unzip it to your desired location.
    * The structure should be:
        ```
        your_folder/
        ├── index.html
        └── assets/
            └── your_image.jpg
            └── another_image.jpg
        ```
    * Open the `index.html` file directly in your web browser.
    * If you add images, make sure you update the code in the .html file with those image locations!

## Feedback, Issues & Feature Requests

Have feedback or have an idea for a new feature? Please use **GitHub Discussions**!

1.  **Go to Discussions:** Navigate to the [Discussions](https://github.com/warframe-tools/Task-Checklist/discussions) tab of this repository.
2.  **Choose a Category:** Select the most appropriate category (e.g., "Ideas" for feature requests, "Q&A" for questions, "General" for feedback, or create a new discussion if unsure).
3.  **Start Discussion:** Click "New discussion".
4.  **Describe:**
    * Provide a clear and concise title.
    * **For Bugs:** Describe the steps to reproduce the issue, what you expected, what happened, and paste any error messages (use the "Copy" button in the app's error bar if available). Include browser/OS info if possible.
    * **For Features:** Explain the feature clearly and why it would be useful.
    * **For Feedback:** Share your thoughts!
5.  **Submit:** Click "Start discussion".

## Reporting Issues (Bugs)

If you encounter a bug, graphical glitch, or something isn't working as expected, please report it using the **GitHub Issue Tracker**:

1.  **Check for Existing Issues:** First, please check the [Issues](https://github.com/warframe-tools/Task-Checklist/issues) tab to see if someone has already reported the same problem.
2.  **New Issue:** If not, click "New issue".
3.  **Describe the Bug:**
    * Provide a clear and concise title (e.g., "Weekly Reset Button Doesn't Reset All Weekly Tasks").
    * Describe the exact steps you took to encounter the bug.
    * What did you expect to happen?
    * What actually happened?
    * **Paste any error messages** shown in the app's error bar (use the "Copy" button) or from your browser's developer console.
    * Include your browser name and version, and operating system if possible.
4.  **Submit:** Click "Submit new issue".

## Support the Project

If you find this tool useful, consider supporting its development!

* **GitHub Sponsors:** You can sponsor this project via the [Sponsor](https://github.com/sponsors/warframe-tools) button on the repository page.
* **Create a Pull Request:** Do you have a feature you would like added, or a task that you would like added that could benefit other Tenno? Fork the repository, and create a pull request!

## Credits

* **Tailwind CSS:** [https://tailwindcss.com/](https://tailwindcss.com/)
* **Inter Font:** [https://fonts.google.com/specimen/Inter](https://fonts.google.com/specimen/Inter)
* Task list based on information discussed in the Warframe community.

## Disclaimer

This is an unofficial fan-made tool. Warframe and all related assets are the intellectual property of Digital Extremes Ltd. This project is not affiliated with, endorsed by, or sponsored by Digital Extremes Ltd.

> [!NOTE] 
> The warframetools.com website uses [**Cloudflare Analytics**](https://www.cloudflare.com/web-analytics/) to view privacy friendly analytics information for visitors. You are free to use a tracker blocker, and it will not affect the tool from working. If you are not comfortable with this, please download and use it locally, or fork the repository and host it yourself on your own [Github Pages](https://pages.github.com/).

## License

This project is licensed under the **GNU General Public License v3.0 (GPLv3)**. See the [LICENSE](https://github.com/warframe-tools/Task-Checklist?tab=GPL-3.0-1-ov-file) file for details.