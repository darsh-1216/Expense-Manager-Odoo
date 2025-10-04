# Smart Expense Management System

A comprehensive, multi-page expense management prototype built with React, TypeScript, and Tailwind CSS. This system demonstrates role-based access control, multi-level approval workflows, OCR simulation, and currency conversion features.

## 🌟 Features

### Core Functionality
- **Role-Based Access Control**: Different dashboards for Employees, Managers, and Admins
- **Multi-Level Approval Workflow**: Configurable approval chains with conditional rules
- **Expense Management**: Submit, track, and manage expense reports
- **Receipt Management**: Upload and store receipt images
- **Real-Time Analytics**: Visual dashboards with expense summaries

### Special Features
- **OCR Simulation**: Upload receipts for automatic text extraction and form auto-filling
- **Currency Converter**: Real-time currency conversion for international expenses
- **Visual Approval Flow**: Track expense approval progress through multiple steps
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

### User Roles
- **Employee**: Submit expenses, view history, track approval status
- **Manager**: Review and approve/reject team expenses, view team analytics
- **Admin**: Manage users, configure approval rules, view all expenses

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone or download the project**
   ```bash
   cd smart-expense-management
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   Navigate to `http://localhost:3000`

## 🔐 Demo Accounts

Use these pre-configured accounts to explore different user roles:

### Admin Account
- **Email**: admin@demo.com
- **Password**: password123
- **Access**: Full system access, user management, approval rules

### Manager Account
- **Email**: manager@demo.com
- **Password**: password123
- **Access**: Team expense management, approval workflows

### Employee Account
- **Email**: employee@demo.com
- **Password**: password123
- **Access**: Expense submission, history tracking

## 📱 Demo Flow

### Recommended Testing Sequence

1. **Start as Employee**
   - Login with employee@demo.com / password123
   - Submit a new expense with receipt upload
   - View expense history and approval status

2. **Switch to Manager**
   - Login with manager@demo.com / password123
   - Review pending approvals
   - Approve or reject expenses with comments

3. **Access as Admin**
   - Login with admin@demo.com / password123
   - View all expenses and system analytics
   - Configure approval rules

4. **Test Special Features**
   - Try OCR Simulation with receipt upload
   - Use Currency Converter for multi-currency expenses
   - Explore visual approval flow tracking

## 🛠️ Technology Stack

### Frontend
- **React 18**: Modern React with hooks and functional components
- **TypeScript**: Type-safe JavaScript development
- **Tailwind CSS**: Utility-first CSS framework
- **React Router**: Client-side routing

### UI Libraries
- **Recharts**: Data visualization and charts
- **Heroicons**: Beautiful SVG icons

### Data Management
- **Local Storage**: Client-side data persistence
- **Mock APIs**: Simulated backend functionality
- **Context API**: State management for authentication

## 📁 Project Structure

```
smart-expense-management/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Layout.tsx
│   │   ├── Navbar.tsx
│   │   └── ProtectedRoute.tsx
│   ├── contexts/
│   │   └── AuthContext.tsx
│   ├── data/
│   │   └── mockData.ts
│   ├── pages/
│   │   ├── Home.tsx
│   │   ├── Login.tsx
│   │   ├── Dashboard.tsx
│   │   ├── SubmitExpense.tsx
│   │   ├── ExpenseHistory.tsx
│   │   ├── PendingApprovals.tsx
│   │   ├── OCRSimulation.tsx
│   │   ├── CurrencyConverter.tsx
│   │   └── About.tsx
│   ├── types/
│   │   └── index.ts
│   ├── utils/
│   │   ├── storage.ts
│   │   └── currency.ts
│   ├── App.tsx
│   ├── index.tsx
│   └── index.css
├── package.json
├── tailwind.config.js
├── tsconfig.json
└── README.md
```

## 🎯 Key Components

### Authentication System
- Role-based login with demo accounts
- Protected routes based on user permissions
- Session management with local storage

### Expense Management
- **Submit Expense**: Form with validation, receipt upload, category selection
- **Expense History**: Filterable list with approval status tracking
- **Pending Approvals**: Manager interface for reviewing and approving expenses

### Special Features
- **OCR Simulation**: Mock receipt processing with extracted data
- **Currency Converter**: Real-time exchange rate simulation
- **Approval Flow**: Visual progress tracking through multiple approval steps

### Dashboard Analytics
- Expense statistics and summaries
- Approval status counts
- Quick action buttons for common tasks

## 🔧 Configuration

### Environment Setup
The application uses local storage for data persistence. All demo data is pre-loaded and resets on each session.

### Customization
- **Colors**: Modify `tailwind.config.js` for custom color schemes
- **Data**: Update `src/data/mockData.ts` for different sample data
- **Routes**: Add new pages in `src/pages/` and update `App.tsx`

## 📊 Sample Data

The system includes pre-loaded demo data:
- **Users**: 4 demo accounts with different roles
- **Expenses**: Sample expense submissions with various statuses
- **Categories**: Common expense categories (Travel, Meals, Office Supplies, etc.)
- **Approval Rules**: Configurable approval workflows
- **Currency Rates**: Mock exchange rates for major currencies

## 🎨 Design Features

### Responsive Design
- Mobile-first approach with Tailwind CSS
- Adaptive layouts for different screen sizes
- Touch-friendly interface elements

### Accessibility
- WCAG-compliant color contrasts
- Keyboard navigation support
- Screen reader-friendly markup

### User Experience
- Intuitive navigation with role-based menus
- Clear visual feedback for user actions
- Loading states and error handling
- Smooth transitions and animations

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Serve Locally
```bash
npx serve -s build
```

### Deploy to Static Hosting
The built application can be deployed to any static hosting service:
- Vercel
- Netlify
- GitHub Pages
- AWS S3
- Firebase Hosting

## 🤝 Contributing

This is a demonstration prototype. For production use, consider:
- Implementing a real backend API
- Adding proper authentication with JWT tokens
- Integrating real OCR services
- Connecting to live currency exchange APIs
- Adding comprehensive error handling
- Implementing proper data validation

## 📄 License

This project is created for demonstration purposes. Feel free to use and modify for your own projects.

## 🆘 Support

For questions or issues with the demo:
- Check the About page for demo information
- Review the README for setup instructions
- Ensure all dependencies are properly installed

---

**Note**: This is a demonstration prototype with simulated data. All financial amounts, exchange rates, and user data are for showcase purposes only.
