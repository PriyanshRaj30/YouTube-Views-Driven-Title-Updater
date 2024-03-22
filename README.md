**YouTube Video Details Updater**

This script is designed to automatically update the details of a YouTube video if certain validation criteria are not met. It utilizes the YouTube Data API to retrieve video details and update them accordingly.

### How it Works

The `main()` function serves as the entry point. It sets the `videoId` variable to the ID of the target YouTube video and retrieves its details using the `getVideoDetails()` function. If the video details fail to pass the validation criteria specified in the `validate()` function, the details are updated via the `updateDetails()` function.

### Functions

1. **main()**: Entry point of the script. It retrieves video details and validates them. If validation fails, it updates the details.
   
2. **getVideoDetails(videoId)**: Retrieves details of the specified YouTube video using the YouTube Data API. It fetches the video's title, category ID, and view count.

3. **validate(videoData)**: Checks whether the video details meet certain validation criteria. In this script, it checks if the video title contains the view count. If the validation fails, it returns false.

4. **updateDetails(videoData)**: Updates the video details if the validation fails. It constructs a new title for the video based on its current view count and updates the video's title and category ID using the YouTube Data API.

### Usage

1. **Set Up Google Cloud Project**: Before using the script, you need to create a Google Cloud project and enable the YouTube Data API for it. Follow the instructions provided by Google to set up your project and obtain API credentials.

2. **Install Google Apps Script**: Copy the provided code into a Google Apps Script project. Save the project and give it an appropriate name.

3. **Replace Placeholder**: Replace `"VIDEOID"` in the `videoId` variable with the ID of the target YouTube video.

4. **Set Up Trigger**: To automate the script, set up a trigger in Google Apps Script. Go to the "Triggers" menu, click on "Add Trigger", select the `main()` function, choose the event type (e.g., time-driven), and set the desired interval for the script to run.

5. **Run the Script**: Run the `main()` function to execute the script manually for the first time. After setting up the trigger, the script will run automatically based on the specified interval.

### Requirements

- Google account with access to Google Apps Script.
- Google Cloud project with YouTube Data API enabled.
- Proper authorization to access and modify YouTube video details.

### License

This script is provided under the MIT License. Feel free to use and modify it according to your needs.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request to suggest improvements or additional features.

## Author

👤 **Priyanshu Raj**

* Github: [@PriyanshRaj30](https://github.com/PriyanshRaj30)

## Support
- Give a ⭐️ if this project helped you!
- If you encounter any issues or have questions about using the script, please [open an issue](https://github.com/PriyanshRaj30/yt-thumbnail-stats/issues) on GitHub.

---
