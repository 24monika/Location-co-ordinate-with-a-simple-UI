 Location-co-ordinate-with-a-simple-UI
Phone Number Tracker

This Python application allows users to track the geographical location and carrier information of a phone number. Additionally, it generates a map of the phone number's location and provides a button to view the location in a web browser.

---

Requirements
1. Python Version: Ensure Python 3.x is installed.
2. Python Libraries: Install the following libraries before running the application:
   ```bash
   pip install phonenumbers opencage folium
   ```
3. Files:
   - `logo.png`: A logo image for the GUI.
   - `search_icon.png`: A search button icon.

4. API Key:  
   - Replace `"c683e23dd4d642db8559f0256d9b6aec"` with your valid OpenCage Geocoding API key.

---

 Setup Instructions
1. Clone or download the project.
2. Ensure all dependencies are installed.
3. Place the `logo.png` and `search_icon.png` files in the same directory as the script.
4. Replace the placeholder OpenCage API key with your valid key.
5. Run the script using:
   ```bash
   python phone_tracker.py
   ```

---

 How to Use
1. Launch the application.
2. Enter a phone number in the input field.
3. Click the search icon to fetch the location and carrier information.
4. If successful, a map file `myLocation.html` is generated.
5. Click "View Location" to open the map in your default web browser.

---

Code Overview
1. Dependencies:
   - `phonenumbers`: For phone number parsing and validation.
   - `opencage`: For fetching geographical coordinates.
   - `folium`: For generating an interactive map.
   - `tkinter`: For GUI components.
   - `webbrowser`: For opening the generated map.

2. Main Functions:
   - `track()`: 
     - Parses the phone number.
     - Fetches location and carrier details.
     - Generates the map using Folium.
   - `open_map()`: Opens the generated HTML map in a web browser.

3. GUI Layout:
   - Includes input fields, labels for location and carrier, and buttons for map actions.

---

Limitations
- Accuracy: Relies on the OpenCage Geocoding API for location accuracy.
- Input Validation: Only valid phone numbers with international codes are accepted.
- Dependencies: Requires an active internet connection for API requests.

---

 Future Enhancements
- Add error handling for invalid API responses.
- Support multiple languages for location descriptions.
- Improve the GUI layout for better user experience.

---

License
This project is licensed under the MIT License. Feel free to modify and use it as per your requirements.
