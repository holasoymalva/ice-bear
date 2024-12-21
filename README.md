# ❄️ Ice Bear

A powerful, Streamlit-inspired library for building data applications in Node.js. Ice Bear makes it easy to create beautiful, interactive data dashboards and applications with minimal code.

## 🚀 Features

- **Simple API**: Create complex data applications with minimal code
- **Interactive Components**: Built-in widgets like buttons, sliders, and input fields
- **Data Visualization**: Easy-to-use charts and graphs powered by modern visualization libraries
- **Layouts**: Flexible layout system with columns and sidebars
- **State Management**: Built-in state management for reactive applications
- **Real-time Updates**: Support for real-time data updates and streaming
- **Responsive Design**: Mobile-first approach for all components

## 📦 Installation

```bash
npm install ice-bear
```

## 🎯 Quick Start

```javascript
const ice = require('ice-bear');

// Create a simple dashboard
async function createDashboard() {
  ice.header('My Dashboard');
  
  const [count, setCount] = ice.useState(0);
  
  ice.button('Click me!', () => setCount(count + 1));
  ice.text(`Button clicked ${count} times`);
  
  ice.lineChart({
    data: yourData,
    x: 'date',
    y: 'value',
    title: 'Trending Data'
  });
}

createDashboard();
```

## 📚 Documentation

### Core Components

#### Text and Headers
```javascript
ice.text('Simple text');
ice.header('Main Title', 1);
ice.markdown('**Bold** and *italic* text');
```

#### Data Display
```javascript
ice.dataframe(data);
ice.table(data);
ice.json(data);
```

#### Charts
```javascript
ice.lineChart(data, options);
ice.barChart(data, options);
ice.scatterPlot(data, options);
```

#### Interactive Elements
```javascript
ice.button('Click me', onClick);
ice.slider(0, 100, defaultValue);
ice.input('Enter text', onChange);
```

#### Layout
```javascript
const [col1, col2] = ice.columns(2);
const sidebar = ice.sidebar();
```

## 🛣️ Roadmap

### Phase 1: Core Features (In Progress)
- [x] Basic component system
- [x] State management
- [x] Layout components
- [ ] Theme system
- [ ] Error handling improvements

### Phase 2: Enhanced Visualization (Planned)
- [ ] Additional chart types
  - [ ] Pie charts
  - [ ] Area charts
  - [ ] Candlestick charts
- [ ] Custom themes for charts
- [ ] Animation support
- [ ] Interactive tooltips

### Phase 3: Advanced Features (Planned)
- [ ] Real-time data streaming
- [ ] WebSocket support
- [ ] Data caching system
- [ ] Export functionality
  - [ ] PDF export
  - [ ] CSV export
  - [ ] Image export

### Phase 4: Developer Experience (Planned)
- [ ] CLI tool for project scaffolding
- [ ] Developer tools and debugging
- [ ] Performance optimization
- [ ] Testing utilities

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/ice-bear.git

# Install dependencies
npm install

# Run tests
npm test

# Build the library
npm run build
```

## 📝 Testing

```bash
# Run all tests
npm test

# Run specific test suite
npm test -- --grep "Component Tests"

# Run tests with coverage
npm run test:coverage
```

## 🔑 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤔 FAQ

**Q: How does Ice Bear compare to Streamlit?**
A: Ice Bear brings Streamlit's intuitive API and rapid development capabilities to the Node.js ecosystem, while adding features specific to JavaScript and web development.

**Q: Can I use Ice Bear with existing Node.js applications?**
A: Yes, Ice Bear can be integrated into existing Express.js or other Node.js applications.

**Q: Is Ice Bear suitable for production use?**
A: Ice Bear is currently in early development. While it's great for prototypes and internal tools, we're working towards production readiness.

## 🙏 Acknowledgments

- Inspired by Streamlit's excellent design and API
- Built with modern JavaScript features
- Powered by the Node.js ecosystem

## 📞 Support

- Create an issue for bug reports
- Join our Discord community for discussions
- Check out the documentation for detailed guides
- Follow us on Twitter for updates

---

Built with ❄️ by the Ice Bear Team
