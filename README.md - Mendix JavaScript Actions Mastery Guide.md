
# Mendix Mastery Series: JavaScript Actions 📚

[![Mendix](https://img.shields.io/badge/Mendix-Compatible-blue.svg)](https://mendix.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-Educational-green.svg)](#)
[![Author](https://img.shields.io/badge/Author-Mendix%20MVP-purple.svg)](#author)

> **From Basic Operations to AI Integration and Data Visualization**  
> A comprehensive guide to mastering JavaScript Actions in Mendix applications

## 📖 About This Repository

This repository contains the complete source code, examples, and practical implementations from **"Mendix Mastery Series: JavaScript Actions - Book 1"** by Quang Nhat Tran, Mendix Certified Expert Developer & MVP.

### 🎯 What You'll Learn

Transform from a basic Mendix developer to a JavaScript Action expert capable of implementing enterprise-grade solutions through three comprehensive, production-ready projects.

## 📋 Table of Contents

- [🚀 Getting Started](#getting-started)
- [📚 Book Structure](#book-structure)
- [🛠️ Prerequisites](#prerequisites)
- [💻 Installation](#installation)
- [🎓 Learning Path](#learning-path)
- [📁 Project Structure](#project-structure)
- [🔧 Usage Examples](#usage-examples)
- [🤖 AI Integration](#ai-integration)
- [📊 Data Visualization](#data-visualization)
- [🏗️ Best Practices](#best-practices)
- [🐛 Troubleshooting](#troubleshooting)
- [📞 Support](#support)
- [👨‍💻 Author](#author)

## 🚀 Getting Started

### Quick Start Checklist
- [ ] Mendix Studio Pro installed (latest version recommended)
- [ ] Basic understanding of Mendix platform
- [ ] JavaScript fundamentals (helpful but not required)
- [ ] OpenAI API key (for AI chat examples)
- [ ] Node.js installed (for ECharts integration)

## 📚 Book Structure

### **Topic I: Overview of JavaScript** 🌟
**Master the fundamentals of Mendix JavaScript Actions**

#### I.I Basic Operations
- **Simple Alert Action** - Interactive user messaging with `mx.ui.info()`
- **Logging Action** - Comprehensive debugging and error tracking

#### I.II DOM Manipulation
- **Dynamic Element Creation** - Real-time HTML element generation
- **Element Style Modification** - Advanced CSS manipulation and styling

#### I.III Data Handling
- **Data Transformation** - Array processing and calculated fields
- **External API Integration** - HTTP requests with authentication
- **POST/GET Operations** - Complete REST API interaction patterns

#### I.IV Advanced Techniques
- **Memoization** - Performance optimization through caching
- **Date Formatting** - Professional date/time handling
- **Error Handling** - Enterprise-grade error management

### **Topic II: Real-Time AI Chat with Streaming Responses** 🤖
**Build ChatGPT-like streaming interfaces in Mendix**

#### Key Features:
- ✅ **OpenAI API Integration** with streaming responses
- ✅ **Server-Sent Events (SSE)** for real-time communication
- ✅ **Professional UI** with modern popup design
- ✅ **Database Persistence** using Mendix data APIs
- ✅ **Smart Textarea Detection** with multiple fallback strategies
- ✅ **Auto-close Functionality** with countdown timer

#### Technical Highlights:
```javascript
// Real-time streaming processing
const reader = response.body.getReader();
const decoder = new TextDecoder();
// Process chunks and update UI dynamically
```

### **Topic III: Dynamic Charts with Apache ECharts** 📊
**Create interactive data visualizations**

#### Chart Types Supported:
- 🥧 **Pie Charts** - Distribution visualization
- 🍩 **Doughnut Charts** - Hollow pie charts with center labels
- 🫧 **Bubble Charts** - Multi-dimensional data representation
- 📈 **Scatter Plots** - Correlation and trend analysis

#### Key Features:
- ✅ **NPM Integration** - Offline ECharts library management
- ✅ **Dynamic Chart Switching** - Runtime chart type changes
- ✅ **Instance Management** - Memory optimization
- ✅ **Responsive Design** - Mobile and desktop compatibility

## 🛠️ Prerequisites

### Mendix Environment
```
Mendix Studio Pro: 9.18+ (recommended)
Mendix Runtime: Compatible with latest LTS
Browser Support: Chrome, Firefox, Safari, Edge
```

### Development Tools
```
Node.js: 16+ (for ECharts integration)
npm: 8+ (package management)
Git: Latest (version control)
```

### API Requirements
```
OpenAI API Key (for AI chat features)
Internet connection (for API calls)
```

## 💻 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/mendix-javascript-actions-mastery.git
cd mendix-javascript-actions-mastery
```

### 2. Install Dependencies (for ECharts)
```bash
npm install echarts
```

### 3. Mendix Project Setup
```bash
# Import the .mpk file into your Mendix project
# Or copy JavaScript actions to your existing project
```

### 4. Environment Configuration
```javascript
// Set your OpenAI API key in constants
OPENAI_API_KEY: "your-api-key-here"
OPENAI_MODEL: "gpt-4" // or your preferred model
```

## 🎓 Learning Path

### **Beginner Level** (1-2 weeks)
1. **Start with Topic I** - Basic Operations
2. **Practice DOM Manipulation** - Build interactive elements
3. **Master Error Handling** - Professional debugging

### **Intermediate Level** (2-3 weeks)
1. **Data Transformation** - Advanced array processing
2. **API Integration** - External service communication
3. **Performance Optimization** - Memoization techniques

### **Advanced Level** (3-4 weeks)
1. **AI Chat Implementation** - Streaming responses
2. **Dynamic Visualizations** - ECharts integration
3. **Production Deployment** - Enterprise patterns

## 📁 Project Structure

```
mendix-javascript-actions/
├── 📁 Topic1-BasicOperations/
│   ├── 🟨 JS_SimpleAlertAction.js
│   ├── 🟨 JS_LoggingAction.js
│   ├── 🟨 JS_DynamicEventCreation.js
│   ├── 🟨 JS_ModifyElementStyle.js
│   └── 🟨 JS_TransformData.js
│
├── 📁 Topic2-AIChat/
│   ├── 🟨 JS_StreamOpenAIResponse.js
│   ├── 📄 StreamingResponse_NewEdit.page.xml
│   ├── 🗃️ Domain-Model.xml
│   └── 📋 README-AIChat.md
│
├── 📁 Topic3-DataVisualization/
│   ├── 🟨 JS_InitializeChart.js
│   ├── 🟨 JS_DynamicChart.js
│   ├── 📦 package.json
│   └── 📋 README-Charts.md
│
├── 📁 examples/
│   ├── 🎯 basic-examples.md
│   ├── 🤖 ai-chat-examples.md
│   └── 📊 chart-examples.md
│
├── 📁 docs/
│   ├── 🔧 installation-guide.md
│   ├── 🏗️ best-practices.md
│   └── 🐛 troubleshooting.md
│
└── 📖 README.md
```

## 🔧 Usage Examples

### Basic Alert Action
```javascript
// Simple user notification
export async function JS_SimpleAlertAction(userMessage) {
    mx.ui.info(userMessage, {
        modal: true,
        blocking: true
    });
    return true;
}
```

### Dynamic Element Creation
```javascript
// Create animated elements
export async function JS_DynamicEventCreation(containerClass, elementType, content, animationType) {
    const container = document.querySelector('.' + containerClass);
    const element = document.createElement(elementType);
    
    // Apply animations and styling
    element.style.cssText = `
        opacity: 0;
        transform: scale(0.8);
        transition: all 0.5s ease-in-out;
    `;
    
    // Add to DOM and animate
    container.appendChild(element);
    setTimeout(() => {
        element.style.opacity = '1';
        element.style.transform = 'scale(1)';
    }, 100);
}
```

### Data Transformation
```javascript
// Transform and enhance data
export async function JS_TransformData(inputData) {
    const data = JSON.parse(inputData);
    
    const transformedData = data.map(item => ({
        ...item,
        fullName: `${item.firstName} ${item.lastName}`,
        age: calculateAge(item.birthDate),
        salaryGrade: item.salary >= 55000 ? 'High' : 'Standard'
    }));
    
    return JSON.stringify(transformedData, null, 2);
}
```

## 🤖 AI Integration

### Streaming Chat Implementation

#### Key Components:
1. **OpenAI API Integration**
2. **Real-time Response Processing**
3. **Dynamic UI Updates**
4. **Database Persistence**

#### Example Usage:
```javascript
// Initialize streaming chat
JS_StreamOpenAIResponse(userMessage, sessionChatGuid)
    .then(response => {
        console.log('Chat completed successfully');
    })
    .catch(error => {
        console.error('Chat failed:', error);
    });
```

#### Features:
- ✨ **Real-time streaming** - See responses as they generate
- 💾 **Auto-save** - Conversation history persisted
- 🎨 **Professional UI** - Modern popup design
- 📱 **Responsive** - Works on all device sizes

## 📊 Data Visualization

### ECharts Integration

#### Supported Chart Types:
```javascript
// Dynamic chart creation
const chartTypes = {
    'pie': 'Distribution visualization',
    'doughnut': 'Hollow center charts', 
    'bubble': 'Multi-dimensional data',
    'scatter': 'Correlation analysis'
};
```

#### Example Implementation:
```javascript
// Initialize chart
var chartDom = document.getElementsByClassName('airefine')[0];
var myChart = echarts.init(chartDom);

// Dynamic chart switching
switch(chartType.toLowerCase()) {
    case 'pie chart':
        option = {
            title: { text: 'Population Distribution' },
            series: [{
                type: 'pie',
                data: transformedData
            }]
        };
        break;
}

myChart.setOption(option);
```

## 🏗️ Best Practices

### ✅ Do's
- **Keep actions focused** - Single responsibility principle
- **Use async/await** - Modern asynchronous patterns
- **Implement error handling** - Comprehensive try-catch blocks
- **Validate inputs** - Always check parameters
- **Log appropriately** - Use structured logging

### ❌ Don'ts
- **Avoid complex logic** - Keep JavaScript actions lightweight
- **Don't ignore errors** - Always handle failure scenarios
- **No global variables** - Use proper scoping
- **Don't manipulate entities directly** - Use Mendix APIs

### 🔒 Security Considerations
```javascript
// Always validate inputs
if (!userMessage || typeof userMessage !== 'string') {
    console.error('Invalid input parameter');
    return false;
}

// Sanitize user content
const sanitizedContent = userMessage.replace(/<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi, '');
```

## 🐛 Troubleshooting

### Common Issues & Solutions

#### **Issue**: JavaScript Action not executing
```javascript
// Check console for errors
console.log('Action started:', new Date().toISOString());

// Verify container exists
const container = document.querySelector('.' + containerClass);
if (!container) {
    console.error('Container not found:', containerClass);
    return false;
}
```

#### **Issue**: API calls failing
```javascript
// Add proper error handling
try {
    const response = await fetch(apiUrl, {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
            'Authorization': `Bearer ${apiKey}`
        },
        body: JSON.stringify(payload)
    });
    
    if (!response.ok) {
        throw new Error(`HTTP ${response.status}: ${response.statusText}`);
    }
    
} catch (error) {
    console.error('API call failed:', error);
    mx.ui.error(`API Error: ${error.message}`);
}
```

#### **Issue**: ECharts not rendering
```javascript
// Ensure DOM element exists
const chartDom = document.getElementsByClassName('chart-container')[0];
if (!chartDom) {
    console.error('Chart container not found');
    return;
}

// Check if ECharts is loaded
if (typeof echarts === 'undefined') {
    console.error('ECharts library not loaded');
    return;
}
```

### Debug Mode
```javascript
// Enable detailed logging
const DEBUG_MODE = true;

function debugLog(message, data = null) {
    if (DEBUG_MODE) {
        console.log(`[DEBUG] ${message}`, data);
    }
}
```

## 📞 Support

### 📧 Contact Information
- **Author**: Quang Nhat Tran
- **Title**: Mendix Certified Expert Developer & MVP
- **Role**: Senior Technical Lead - Solution Architect
- **Location**: Bangkok, Thailand

### 🔗 Resources
- **Book**: Available for purchase
- **Complete Project Files**: Included with book purchase
- **Video Tutorials**: Coming soon
- **Community Forum**: Join our Discord server

### 🆘 Getting Help

1. **Check Documentation** - Review relevant sections
2. **Search Issues** - Look for similar problems
3. **Console Logs** - Enable debug mode
4. **Create Issue** - Provide detailed description

### 📝 Issue Template
```markdown
**Environment:**
- Mendix Version: [e.g., 9.18.4]
- Browser: [e.g., Chrome 120]
- JavaScript Action: [e.g., JS_StreamOpenAIResponse]

**Description:**
[Clear description of the issue]

**Steps to Reproduce:**
1. Step 1
2. Step 2
3. Step 3

**Expected vs Actual:**
Expected: [what should happen]
Actual: [what actually happened]

**Console Errors:**
[paste any console errors]
```

## 👨‍💻 Author

### Quang Nhat Tran
**Mendix Certified Expert Developer & MVP**

With 17+ years in software development and extensive expertise in Mendix platform since 2016, Quang Nhat Tran brings enterprise-grade solutions to the low-code community.

#### 🏆 Credentials
- **Mendix Certified Expert Developer** (Highest certification level)
- **Mendix MVP** (2021-2023, 2025+)
- **