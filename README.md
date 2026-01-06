# 📍 Phone Number Location Tracker

A Python-based tool that tracks the geographical location of a phone number and visualizes it on an interactive map.

## 🌟 Features

- Extract country/region information from phone numbers
- Identify carrier/service provider
- Get geographical coordinates (latitude and longitude)
- Generate an interactive map with location marker
- Export map as HTML file

## 🛠️ Technologies Used

- **phonenumbers** - Phone number parsing and validation
- **opencage** - Geocoding API for coordinate conversion
- **folium** - Interactive map generation with Leaflet.js

## 📋 Prerequisites

Before running this project, make sure you have Python installed on your system.

## 🚀 Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/phone-location-tracker.git
cd phone-location-tracker
```

2. Install required dependencies:
```bash
pip install phonenumbers
pip install opencage
pip install folium
```

## 🔑 API Key Setup

This project uses OpenCage Geocoding API. You'll need to:

1. Sign up for a free API key at [OpenCage](https://opencagedata.com/)
2. Replace the API key in `location_tracker.py`:
```python
key = 'YOUR_API_KEY_HERE'
```

## 💻 Usage

1. Open `location_tracker.py` and modify the phone number:
```python
number = "+8801973445094"  # Replace with your target number
```

2. Run the script:
```bash
python location_tracker.py
```

3. The script will:
   - Print the country/region
   - Print the carrier name
   - Print the coordinates (latitude, longitude)
   - Generate `mylocation.html` with an interactive map

4. Open `mylocation.html` in your web browser to view the location on the map.

## 📁 Project Structure

```
phone-location-tracker/
│
├── location_tracker.py    # Main Python script
├── mylocation.html        # Generated map output
└── README.md             # Project documentation
```

## 🔍 How It Works

1. **Phone Number Parsing**: Uses the `phonenumbers` library to parse and validate the phone number
2. **Location Extraction**: Extracts country/region information from the phone number
3. **Carrier Detection**: Identifies the mobile carrier/service provider
4. **Geocoding**: Converts location name to geographical coordinates using OpenCage API
5. **Map Generation**: Creates an interactive map with Folium and marks the location

## ⚠️ Important Notes

- This tool provides approximate location based on phone number country code and region
- Accuracy depends on the phone number format and available data
- The location shown is typically the country or region, not the exact GPS location
- Respect privacy laws and regulations in your jurisdiction
- This tool is for educational purposes only

## 📝 Example Output

```
Bangladesh
Grameenphone
24.4769288 90.2934413
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

  Shofi Ahmed
- GitHub: [@shofiahmed69](https://github.com/shofiahmed69)

## ⭐ Show your support

Give a ⭐️ if this project helped you!

## 🔗 Acknowledgments

- [phonenumbers](https://github.com/daviddrysdale/python-phonenumbers)
- [OpenCage Geocoding API](https://opencagedata.com/)
- [Folium](https://python-visualization.github.io/folium/)
