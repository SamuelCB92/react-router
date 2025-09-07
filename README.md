# React Router Demo - Portfolio Website

## 🎯 **Learning Objective:**
Demonstrate React Router fundamentals with a multi-page portfolio website.

## 📚 **Concepts Covered:**

### **React Router Setup:**
- `BrowserRouter` - Enables routing functionality
- `Routes` - Container for route definitions
- `Route` - Individual route configuration
- `Link` - Navigation links (replaces `<a>` tags)
- `useLocation` - Hook to get current route info
- `useNavigate` - Hook for programmatic navigation

### **Navigation Patterns:**
- **Declarative Navigation** - Using `<Link>` components
- **Programmatic Navigation** - Using `useNavigate()` hook
- **Active Link Styling** - Highlighting current page
- **Route Parameters** - Dynamic URL segments

### **Multi-Page Application:**
- **Home Page** - Landing page with navigation button
- **About Page** - Information about the developer
- **Projects Page** - Showcase of completed projects
- **Contact Page** - Contact form with state management

## 🚀 **How to Run:**
1. Open `react-router-demo.html` in your browser
2. Navigate between pages using the navigation bar
3. Test the "View My Projects" button (programmatic navigation)
4. Fill out the contact form to see state management

## 🔍 **Key Learning Points:**

### **1. Route Definition:**
```jsx
<Routes>
    <Route path="/" element={<HomePage />} />
    <Route path="/about" element={<AboutPage />} />
    <Route path="/projects" element={<ProjectsPage />} />
    <Route path="/contact" element={<ContactPage />} />
</Routes>
```

### **2. Navigation Links:**
```jsx
<Link to="/projects" className="nav-link">
    Projects
</Link>
```

### **3. Programmatic Navigation:**
```jsx
const navigate = useNavigate();
<button onClick={() => navigate('/projects')}>
    View My Projects
</button>
```

### **4. Active Link Styling:**
```jsx
const location = useLocation();
className={`nav-link ${location.pathname === item.path ? 'active' : ''}`}
```

## 📝 **Next Steps:**
- Add URL parameters (e.g., `/projects/:id`)
- Implement nested routes
- Add route guards (protected routes)
- Learn about route loaders and actions

## 🎓 **Month 4 Progress:**
- ✅ React Hooks (useReducer, useCallback, useMemo, useRef)
- ✅ **React Router** - Multi-page navigation
- ⏳ Controlled forms (next)
- ⏳ API consumption
- ⏳ Project with login + CRUD
