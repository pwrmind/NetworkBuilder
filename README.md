# Brain.js NetworkBuilder

An interactive web-based tool for learning and experimenting with machine learning concepts using Brain.js. This Single Page Application (SPA) provides a visual interface for building, training, and testing various neural network models without writing code.

![Brain.js ML Constructor](https://img.shields.io/badge/Brain.js-ML%20Constructor-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Version](https://img.shields.io/badge/version-1.0.0-orange)

## 🌟 Features

### 🧠 Multiple Neural Network Types
- **Feedforward Networks**: NeuralNetwork, NeuralNetworkGPU
- **Recurrent Networks**: RNN, LSTM, GRU
- **Time Series Networks**: RNNTimeStep, LSTMTimeStep, GRUTimeStep
- **Autoencoders**: AE for unsupervised learning

### 🎨 Visual Model Builder
- Drag-and-drop inspired layer configuration
- Real-time network architecture visualization
- Interactive hyperparameter tuning
- Automatic model configuration based on data

### 📊 Data Management
- Support for CSV and JSON file formats
- Manual data input with JSON validation
- Built-in sample datasets for each network type
- Automatic data preprocessing and normalization
- Data statistics and visualization

### 🚀 Training & Monitoring
- Real-time training progress visualization
- Interactive error charts using D3.js
- Training logs and performance metrics
- Ability to pause, resume, and stop training
- Cross-validation support

### 🔬 Testing & Analysis
- Interactive model testing interface
- Quality metrics and performance evaluation
- Export trained models and results
- Code generation for reuse

## 🛠 Technologies Used

- **Frontend Framework**: Alpine.js
- **UI Components**: Bootstrap 5 (Compact SM layout)
- **Icons**: Font Awesome 6
- **Typography**: Google Fonts (Inter)
- **Machine Learning**: Brain.js
- **Data Visualization**: D3.js
- **All dependencies loaded via CDN**

## 🚀 Quick Start

### Option 1: Direct File Open
Simply download `index.html` and open it in your browser. No server required!

### Option 2: Local Server
For better performance, run a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 📖 How to Use

### Step 1: Choose Network Type
Select from 8 different neural network types, each with detailed descriptions and use cases.

### Step 2: Configure Model
- Set input/output layer sizes
- Add/remove hidden layers
- Choose activation functions
- Tune hyperparameters (learning rate, momentum, iterations)

### Step 3: Load Data
- Upload CSV/JSON files
- Use built-in sample datasets
- Manual JSON input
- Automatic data preprocessing

### Step 4: Train Model
- Monitor real-time training progress
- View error charts and metrics
- Control training process (pause/resume/stop)

### Step 5: Test & Export
- Test model with custom inputs
- View performance metrics
- Export model as JSON
- Generate reusable JavaScript code

## 🧩 Supported Network Types

| Network Type | Category | Use Cases |
|--------------|----------|-----------|
| NeuralNetwork | Feedforward | Classification, Regression, Pattern Recognition |
| NeuralNetwork GPU | Feedforward | Large datasets, Complex architectures |
| RNN | Recurrent | Time series, Natural language processing |
| LSTM | Recurrent | Machine translation, Text generation |
| GRU | Recurrent | Sentiment analysis, Sequence classification |
| RNN TimeStep | Time Series | Stock prediction, Sensor data analysis |
| LSTM TimeStep | Time Series | Financial forecasting, Medical data |
| Autoencoder | Unsupervised | Data compression, Anomaly detection |

## 📁 Project Structure

```
brainjs-ml-constructor/
│
├── index.html              # Main application file
├── README.md               # Project documentation
│
└── Features:
    ├── Network Type Selection
    ├── Visual Model Configuration
    ├── Data Management
    ├── Training Interface
    ├── Testing & Results
    └── Export Functionality
```

## 🎯 Sample Datasets Included

The application comes with pre-configured sample datasets for each network type:

- **XOR Problem** (Feedforward networks)
- **Sentiment Analysis** (RNN/LSTM/GRU)
- **Time Series Forecasting** (TimeStep networks)
- **Character Classification** (All networks)
- **Math Operations** (Recurrent networks)

## 📋 Export Options

- **Model JSON**: Save trained model configuration and weights
- **JavaScript Code**: Generate ready-to-use Brain.js code
- **Training Results**: Export performance metrics and test results

## 🔧 Customization

### Adding New Network Types
Extend the `networkTypes` array in the JavaScript code:

```javascript
{
    id: 'custom-network',
    name: 'Custom Network',
    category: 'Custom',
    description: 'Your network description',
    sample: {
        data: [...],
        testInput: '...'
    }
}
```

### Modifying UI Components
The application uses Bootstrap's SM breakpoint for compact layout. Modify CSS variables in the style section for custom theming.

## 🌐 Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

### Development Setup
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Brain.js](https://github.com/BrainJS/brain.js) team for the excellent machine learning library
- [Alpine.js](https://alpinejs.dev/) for the lightweight reactivity
- [Bootstrap](https://getbootstrap.com/) for the responsive UI components
- [D3.js](https://d3js.org/) for data visualization capabilities

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](../../issues) page
2. Create a new issue with detailed description
3. Provide browser console logs if applicable

## 🚀 Future Enhancements

- [ ] Model persistence across sessions
- [ ] Advanced visualization of network internals
- [ ] More sample datasets
- [ ] Collaborative features
- [ ] Plugin system for custom networks
- [ ] Performance optimizations for large datasets

---

**Happy Learning with Brain.js!** 🧠✨
