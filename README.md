# SmartVendor AI - Intelligent Inventory Management System

## Overview

SmartVendor AI is a web-based application designed to help street food vendors optimize their inventory management using AI-powered predictions. The system analyzes daily ingredient usage patterns to forecast future needs, reducing waste and preventing stockouts.

## Features

- **AI-Powered Predictions**: Machine learning algorithm that learns from your sales data
- **Mobile-Friendly Interface**: Designed specifically for smartphone use
- **Offline Capability**: Works without internet connection
- **Customizable Ingredients**: Add any ingredients specific to your business
- **Historical Data Tracking**: View past usage patterns
- **Context-Aware Recommendations**: Adjusts predictions based on day of week and vendor type
- **Visual Analytics**: Easy-to-understand interface with animations

## Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript
- **Storage**: LocalStorage for client-side data persistence
- **Libraries**: 
  - Animate.css for animations
  - Font Awesome for icons
  - Google Fonts (Poppins and Montserrat)

## Installation

No installation required! This is a client-side web application that runs directly in the browser. Simply:

1. Open the `index.html` file in any modern web browser
2. The application will work offline after initial load

## Usage Instructions

1. **First-Time Setup**:
   - The app will prompt you to enter your vendor type (e.g., "dosa", "chai", "vada pav")
   
2. **Daily Usage**:
   - Enter the quantities of ingredients you used today
   - Click "Save Today's Usage" to record your data
   - After 3 days of data, you can start getting predictions

3. **Getting Predictions**:
   - Click "Predict Tomorrow's Needs" to get AI-generated shopping list
   - The system will show recommended quantities with confidence indicators

4. **Adding Custom Ingredients**:
   - Click "Add Another Ingredient" to include items specific to your business
   - Enter the name when prompted (e.g., "Paneer", "Special Masala")

## Data Storage

All data is stored locally in the browser using:
- `localStorage.inventoryData` - Stores your daily usage history
- `localStorage.customIngredients` - Stores your custom ingredient list
- `localStorage.vendorType` - Stores your business type

## Customization Options

You can easily customize the app by modifying:

1. **Color Scheme**: Change the CSS variables in the `:root` selector
2. **Default Ingredients**: Modify the form in the HTML to include your common ingredients
3. **Prediction Algorithm**: Adjust the `calculatePrediction()` function in the JavaScript

## Browser Support

The application is tested and works on:
- Chrome (latest)
- Firefox (latest)
- Edge (latest)
- Mobile Chrome and Safari

## Known Limitations

1. Data is only stored locally (will be lost if browser cache is cleared)
2. Predictions improve with more historical data (minimum 3 days recommended)
3. Mobile experience may vary on very small screens

## Future Enhancements

1. Cloud sync capability
2. Multi-language support
3. Advanced analytics dashboard
4. Integration with supplier ordering systems
