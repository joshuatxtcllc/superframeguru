# Frame Guru Master Business Tool

![Frame Guru Master](https://img.shields.io/badge/Version-1.0.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)

A comprehensive business management solution for custom framing companies. This all-in-one application helps you track orders, manage inventory, analyze business metrics, and maintain customer relationships through an intuitive React-based interface.

![Frame Guru Master Dashboard](https://via.placeholder.com/800x450?text=Frame+Guru+Master+Dashboard)

## 🌟 Features

- **Interactive Dashboard**: Visualize order status, material distribution, and business performance
- **Order Management**: Track orders from creation to delivery with status updates
- **Customer Management**: Maintain customer information and order history
- **Inventory Control**: Monitor materials, vendors, and get low stock alerts
- **Dark/Light Mode**: Eye-friendly theme options for comfortable viewing
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **CSV Data Integration**: Easily import your existing frame order data

## 📋 Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)
- A modern web browser

## 🚀 Quick Start

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/frame-guru-master.git

# Navigate to the project directory
cd frame-guru-master

# Install dependencies
npm install

# Start the development server
npm start
```

### Data Setup

1. Place your CSV data file in the `public/data/` directory
2. Name your file `frame-data.csv`
3. Ensure it follows the expected column structure (see Data Format section)

### Deployment

```bash
# Build for production
npm run build

# Deploy to GitHub Pages
npm run deploy
```

## 📊 Data Format

The application expects a CSV file with the following structure:

| Column Name     | Description                                |
|-----------------|--------------------------------------------|
| Order ID        | Unique identifier for each order           |
| Item Number     | Product/SKU identifier                     |
| Vendor          | Provider of framing materials              |
| Customer Name   | Name of the customer                       |
| Material        | Type of material (Moulding, Mat, etc.)     |
| QTY             | Quantity ordered                           |
| Frame Size      | Dimensions of the frame                    |
| Due Date        | Expected completion date                   |
| Order Progress  | Current progress percentage                |
| Ordered         | Boolean (true/false) for Ordered status    |
| Arrived         | Boolean (true/false) for Arrived status    |
| F. Cut          | Boolean (true/false) for Cut status        |
| Prepped         | Boolean (true/false) for Prepped status    |
| Done            | Boolean (true/false) for Done status       |
| Delivered       | Boolean (true/false) for Delivered status  |

## 🎨 Customization

### Business Branding

Edit `src/styles/theme.css` to customize colors:

```css
:root {
  /* Accent colors */
  --accent-teal: #00ADB5;  /* Change to your primary brand color */
  --accent-pink: #E31E6A;  /* Change to your secondary brand color */
  --accent-green: #21C685; /* Change to your tertiary brand color */
}
```

### Custom Components

The modular architecture allows for easy customization of business logic:

- `src/components/Dashboard.js` - Customize metrics and charts
- `src/components/OrderManagement.js` - Modify order workflow
- `src/components/CustomerManagement.js` - Adjust customer fields
- `src/components/InventoryManagement.js` - Customize inventory tracking

## 📱 Mobile View

The Frame Guru Master Business Tool is responsive and works on all devices:

- **Desktop**: Full-featured dashboard with multiple charts
- **Tablet**: Optimized layout with scrollable tables
- **Mobile**: Simplified interface with essential functions

## 🔌 Extending Functionality

### SMS Notifications

The system includes hooks for implementing SMS notifications:

```javascript
// Example implementation with a service like Twilio
const sendSMSNotification = (phone, message) => {
  // Your Twilio integration code here
};
```

### Payment Processing

Add payment processing by connecting to payment gateways:

```javascript
// Example integration with Stripe
const processPayment = (orderId, amount) => {
  // Your payment processing code here
};
```

## 📈 Business Insights

The Frame Guru Master provides valuable insights:

- **Order Trends**: Track completion rates and identify bottlenecks
- **Material Usage**: Monitor material consumption patterns
- **Vendor Analysis**: Compare supplier performance
- **Customer Metrics**: Identify top customers and order patterns

## 🛠️ Technology Stack

- **Frontend**: React.js
- **Charting**: Recharts
- **Data Processing**: PapaParse (CSV), Lodash
- **Styles**: Custom CSS with CSS Variables
- **Deployment**: GitHub Pages / Replit

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📞 Support

For support, feature requests, or bug reports, please open an issue on the repository.

---

Built with ❤️ for custom framing businesses everywhere.
