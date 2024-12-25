# 🏪 Restaurant Payroll System

[![React](https://img.shields.io/badge/React-18.2.0-blue.svg)](https://reactjs.org/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.0-blueviolet.svg)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

A modern, compliant Philippine restaurant payroll management system built with React and TailwindCSS. Designed to handle employee compensation calculations following Philippine labor laws and regulations.

![Payroll System Preview](/api/placeholder/800/400)

## ✨ Features

- 📊 Real-time payroll calculations
- 🔄 Automatic 13th month pay computation (DOLE compliant)
- ⏰ Overtime pay calculation (125% rate)
- 📅 Start date tracking for accurate pro-rating
- ⚡ Input validation and error handling
- 💼 Position-based employee management
- 📱 Responsive design for all devices

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/dagz55/classified-payroll.git
```

2. Install dependencies:
```bash
cd classified-payroll
npm install
```

3. Start the development server:
```bash
npm run dev
```

## 🛠️ Technical Stack

- **Frontend Framework:** React 18
- **Styling:** TailwindCSS
- **UI Components:** shadcn/ui
- **Icons:** Lucide React
- **State Management:** React Hooks

## 📋 System Requirements

- Node.js 16.x or higher
- npm 7.x or higher
- Modern web browser (Chrome, Firefox, Safari, Edge)

## 🎯 Core Functionality

### Employee Management
- Add/edit employee information
- Track start dates
- Manage positions
- Store employee records

### Payroll Calculations
- Basic pay computation
- Overtime pay (125% rate)
- 13th month pay (DOLE compliant)
- Total compensation

### Validation Rules
- Maximum 31 working days per month
- Maximum 72 overtime hours per month
- Negative value prevention
- Required field validation

## 💡 Usage Examples

### Basic Pay Calculation
```javascript
const basicPay = daysWorked * DAILY_RATE;
// Example: 22 days × ₱450 = ₱9,900
```

### Overtime Calculation
```javascript
const overtimePay = overtimeHours * (hourlyRate * 1.25);
// Example: 10 hours × (₱56.25 × 1.25) = ₱703.13
```

### 13th Month Computation
```javascript
const monthlyBasic = DAILY_RATE * AVERAGE_WORKING_DAYS;
const proRated13thMonth = (monthlyBasic / 12) * monthsWorked;
// Example: (₱9,900 / 12) × 6 months = ₱4,950
```

## 🔒 Compliance

This system follows Philippine labor laws and DOLE regulations:
- 13th month pay computation (PD 851)
- Overtime rate calculations (Labor Code Art. 87)
- Basic wage requirements
- Work hour limitations

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support and queries:
- 📧 Email: support@classifiedpayroll.com
- 💬 Issues: GitHub Issues section
- 📚 Documentation: [Wiki](https://github.com/dagz55/classified-payroll/wiki)

---

Made with ❤️ for Philippine Restaurants
