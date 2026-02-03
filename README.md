# School Accounting System - Main Admin Portal

A comprehensive school accounting system with role-based access control for managing students, fees, payments, and reports.

## 🏫 Features

### Student Management
- Student registration with unique ID generation (VMCS0001, VMCS0002, etc.)
- Student search and profile management
- Class-based organization
- Student information updates

### Fee Management
- Individual fee management (add, edit, delete)
- Fee structure management by term and class
- Multiple fee categories (tuition, development, library, sports, laboratory, examination)
- Legacy fee structure support

### Payment Processing
- Payment recording with multiple methods (cash, bank transfer, online)
- Receipt generation and printing
- Payment history tracking
- Outstanding payment management

### Reporting System
- Student fee statements
- Payment reports by term/class
- Outstanding payment tracking
- Fee receipts generation
- Export functionality

### Role-Based Access Control
- **Finance Admin**: Full access - student registration, fee management, payment recording, reports
- **Registrar**: Student registration, search, reports, fee receipts
- **Accountant**: Payment recording, search, reports, fee receipts

## 🚀 Getting Started

### Prerequisites
- Web browser (Chrome, Firefox, Safari, Edge)
- Google Account for backend functionality
- Google Apps Script project

### Setup Instructions

1. **Set up Google Apps Script Backend**
   - Go to [Google Apps Script](https://script.google.com)
   - Create a new project
   - Copy the code from `new.gs` into the script editor
   - Update the `SPREADSHEET_ID` with your Google Sheet ID
   - Deploy as a web app

2. **Configure the Frontend**
   - Update the `scriptURL` in `index-working.html`
   - Replace with your deployed Google Apps Script URL

3. **Create Google Spreadsheet**
   - Create a new Google Spreadsheet
   - The system will automatically create required sheets on first use

## 🔐 Default Login Credentials

- **Email**: admin@school.com
- **Password**: admin123
- **Role**: Finance Admin (or any other role)

## 📁 Files

- `index-working.html` - Main Admin Portal interface
- `new.gs` - Google Apps Script backend
- `README.md` - This documentation

## 🛠️ Usage

1. Open `index-working.html` in your web browser
2. Login with appropriate role credentials
3. Access features based on your role permissions:

### For Finance Admins
- Register new students
- Manage fee structures and individual fees
- Record payments
- Generate all types of reports
- Access all system features

### For Registrars
- Register new students
- Search for students
- Generate reports
- Create fee receipts

### For Accountants
- Record payments
- Search for students
- Generate reports
- Create fee receipts

## 🔧 Configuration

### Backend Configuration
1. Update `SPREADSHEET_ID` in `new.gs` with your Google Sheet ID
2. Deploy Google Apps Script as web app
3. Update `scriptURL` in `index-working.html` with your deployment URL

### Frontend Customization
- Modify role permissions in `rolePermissions` object
- Customize fee categories and classes as needed
- Update school information as required

## 📊 Database Structure

The system uses Google Sheets with these sheets:
- **Students**: Student information and profiles
- **Admins**: Administrator accounts with roles
- **Terms**: Academic terms and periods
- **Fees**: Legacy fee structures
- **IndividualFees**: Individual fee items
- **Payments**: Payment records and transactions

## 🎯 Key Features

### Student Registration
- Automatic ID generation with VMCS prefix
- Class assignment and management
- Parent/guardian information
- Student status tracking

### Fee Management
- Individual fee creation with categories
- Term and class-based fee structures
- Fee editing and deletion
- Real-time fee calculations

### Payment Recording
- Multiple payment methods support
- Receipt generation with unique IDs
- Payment history and tracking
- Outstanding balance calculations

### Reporting
- Comprehensive student statements
- Payment summaries by term/class
- Outstanding payment reports
- Exportable data formats

## 🔒 Security Features

- Role-based access control
- Session management
- Input validation and sanitization
- Secure backend communication

## 🆘 Support

For support:
1. Check Google Apps Script execution logs
2. Verify spreadsheet permissions and structure
3. Ensure proper deployment of the web app
4. Review role permissions and access rights

## 📈 Version History

- **v1.0.0** - Initial admin portal
- **v1.1.0** - Added role-based access control
- **v1.2.0** - Enhanced fee management system
- **v1.3.0** - Individual fee management
- **v1.4.0** - Improved reporting and export features

---

**Main Admin Portal - Developed by BerachahGlobalConcept** 🚀