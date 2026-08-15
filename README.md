# React Components Practice Repository

A comprehensive collection of reusable and customizable React components built for learning and practice purposes. This repository serves as a reference guide for building modern, accessible, and well-structured UI components.

## 📋 Table of Contents

- [Purpose](#purpose)
- [Features](#features)
- [Components](#components)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies](#technologies)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Purpose

This repository is designed to help developers practice and master React component development. It provides a hands-on learning environment for building:

- Reusable UI components
- Component state management
- Props handling and validation
- Responsive design patterns
- Accessibility best practices
- Component composition and modularity

Whether you're a beginner learning the fundamentals or an intermediate developer refining your skills, this repository offers practical examples and implementations.

## ✨ Features

- ✅ **Modular Components** - Independent, reusable components
- ✅ **Responsive Design** - Mobile-first approach across all components
- ✅ **Customizable Props** - Full control over component behavior and styling
- ✅ **Accessible** - Built with accessibility standards in mind
- ✅ **Well Documented** - Clear examples and prop documentation
- ✅ **Clean Code** - Best practices and modern React patterns
- ✅ **No External UI Libraries** - Built from scratch for learning purposes

## 📦 Components

### Navigation Components
- **Navbar** - Responsive navigation bar with menu toggle
- **Sidebar** - Collapsible sidebar navigation with smooth animations
- **Dropdown** - Accessible dropdown menu component

### Layout Components
- **Footer** - Responsive footer with multiple sections

### Data Display Components
- **Cards** - Flexible card component for content display
- **Pagination** - Pagination controls for data navigation

### Form Components
- **Login Form** - User authentication form with validation
- **Signup Form** - User registration form with password confirmation

## 🚀 Installation

### Prerequisites
- Node.js (v14.0 or higher)
- npm or yarn package manager

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/Saravana-2816/react-components.git
cd react-components-practice
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
```

3. **Start the development server**
```bash
npm start
# or
yarn start
```

The application will open at `http://localhost:3000`

## 💡 Usage

### Basic Component Import

```jsx
import Navbar from './components/Navbar';
import Sidebar from './components/Sidebar';
import Card from './components/Card';

function App() {
  return (
    <div className="App">
      <Navbar />
      <Sidebar />
      <Card title="Example Card" description="Component showcase" />
    </div>
  );
}

export default App;
```

### Component Examples

#### Navbar
```jsx
<Navbar 
  logo="My App" 
  menuItems={['Home', 'About', 'Services', 'Contact']}
  onMenuClick={(item) => console.log(item)}
/>
```

#### Sidebar
```jsx
<Sidebar 
  isOpen={sidebarOpen}
  onClose={() => setSidebarOpen(false)}
  items={navigationItems}
/>
```

#### Card
```jsx
<Card 
  title="Component Card"
  description="Learn React components"
  image="/path/to/image.jpg"
  onAction={() => handleAction()}
/>
```

#### Pagination
```jsx
<Pagination 
  currentPage={1}
  totalPages={10}
  onPageChange={(page) => handlePageChange(page)}
/>
```

#### Login Form
```jsx
<LoginForm 
  onSubmit={(credentials) => handleLogin(credentials)}
  onForgotPassword={() => handleForgotPassword()}
/>
```

#### Dropdown
```jsx
<Dropdown 
  options={['Option 1', 'Option 2', 'Option 3']}
  onSelect={(option) => handleSelect(option)}
  placeholder="Select an option"
/>
```

## 📁 Project Structure

```
react-components-practice/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── Navbar/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Navbar.css
│   │   │   └── Navbar.test.jsx
│   │   ├── Sidebar/
│   │   ├── Footer/
│   │   ├── Card/
│   │   ├── Pagination/
│   │   ├── LoginForm/
│   │   ├── SignupForm/
│   │   ├── Dropdown/
│   │   └── index.js
│   ├── pages/
│   │   ├── Home.jsx
│   │   └── ComponentShowcase.jsx
│   ├── styles/
│   │   ├── global.css
│   │   └── variables.css
│   ├── App.jsx
│   ├── App.css
│   └── index.js
├── .gitignore
├── package.json
├── README.md
└── LICENSE
```

## 🛠️ Technologies

- **React 18+** - UI library
- **CSS3** - Styling (with CSS variables for theming)
- **JavaScript ES6+** - Modern JavaScript
- **Node.js** - Runtime environment
- **npm/yarn** - Package management

## 🏃 Getting Started

### For Beginners

1. Start by exploring the `Navbar` and `Card` components
2. Study the component structure and props
3. Modify the styling to understand CSS
4. Add new props and features

### For Intermediate Developers

1. Implement state management with hooks
2. Add form validation to Login/Signup components
3. Create custom hooks for shared logic
4. Implement responsive design patterns
5. Add unit tests for components

### Recommended Learning Path

1. Navigation Components → Navbar, Sidebar, Dropdown
2. Layout Components → Footer, Cards
3. Data Display → Pagination
4. Form Handling → Login, Signup
5. Advanced → Combine multiple components in real-world scenarios

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
```bash
git clone https://github.com/yourusername/react-components-practice.git
```

2. **Create a feature branch**
```bash
git checkout -b feature/new-component
```

3. **Make your changes**
   - Keep components modular and reusable
   - Follow the existing code style
   - Add proper documentation

4. **Commit your changes**
```bash
git commit -m "Add: New component or feature"
```

5. **Push to your branch**
```bash
git push origin feature/new-component
```

6. **Create a Pull Request**
   - Describe your changes clearly
   - Reference any related issues

### Contribution Guidelines

- Write clean, readable code
- Add comments for complex logic
- Follow React best practices
- Ensure components are responsive
- Test components before submitting

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📞 Support

If you have questions or need help:

- Open an **Issue** on GitHub
- Check existing documentation in component folders
- Review component examples in the showcase page

---

**Happy Learning!** 🎉

Feel free to fork this repository, experiment with components, and build amazing UIs with React!