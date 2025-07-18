<div align="center">
  <img src="https://docs.absmartly.com/img/logo.png" alt="ABsmartly Logo" width="200">
  
  # ABsmartly
  
  ### 🚀 The Most Developer-Friendly A/B Testing Platform
  
  [![Website](https://img.shields.io/badge/Website-absmartly.com-blue?style=for-the-badge)](https://www.absmartly.com)
  [![Documentation](https://img.shields.io/badge/Docs-Documentation-green?style=for-the-badge)](https://docs.absmartly.com)
  [![Blog](https://img.shields.io/badge/Blog-Read%20More-orange?style=for-the-badge)](https://www.absmartly.com/blog)
  
</div>

---

## 🎯 What is ABsmartly?

ABsmartly is a powerful, developer-centric A/B testing and feature flagging platform that enables teams to run experiments at scale. Built by developers for developers, it provides the tools and infrastructure needed to make data-driven decisions with confidence.


## ✨ Key Features

<table>
  <tr>
    <td align="center" width="33%">
      <h3>🔬 Advanced Experimentation</h3>
      <p>Run complex multivariate tests with statistical rigor</p>
    </td>
    <td align="center" width="33%">
      <h3>⚡ Real-Time Results</h3>
      <p>See experiment results update in real-time</p>
    </td>
    <td align="center" width="33%">
      <h3>🛡️ Feature Flags</h3>
      <p>Deploy features safely with powerful targeting</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="33%">
      <h3>📊 Statistical Engine</h3>
      <p>Bayesian statistics for accurate results</p>
    </td>
    <td align="center" width="33%">
      <h3>🔌 Easy Integration</h3>
      <p>SDKs for all major languages and frameworks</p>
    </td>
    <td align="center" width="33%">
      <h3>🎨 Visual Editor</h3>
      <p>No-code experiment creation for marketers</p>
    </td>
  </tr>
</table>

## 🛠️ Open Source Projects

### Core SDKs

<div align="center">
  
| SDK | Description | Stars |
|-----|-------------|-------|
| [**Java SDK**](https://github.com/absmartly/java-sdk) | Official Java SDK for ABsmartly | ![Stars](https://img.shields.io/github/stars/absmartly/java-sdk?style=social) |
| [**JavaScript SDK**](https://github.com/absmartly/javascript-sdk) | Browser and Node.js SDK | ![Stars](https://img.shields.io/github/stars/absmartly/javascript-sdk?style=social) |
| [**Go SDK**](https://github.com/absmartly/go-sdk) | Official Go SDK | ![Stars](https://img.shields.io/github/stars/absmartly/go-sdk?style=social) |
| [**Python SDK**](https://github.com/absmartly/python3-sdk) | Python SDK for ABsmartly | ![Stars](https://img.shields.io/github/stars/absmartly/python3-sdk?style=social) |
| [**PHP SDK**](https://github.com/absmartly/php-sdk) | PHP SDK for server-side experiments | ![Stars](https://img.shields.io/github/stars/absmartly/php-sdk?style=social) |
| [**React SDK**](https://github.com/absmartly/react-sdk) | React hooks and components | ![Stars](https://img.shields.io/github/stars/absmartly/react-sdk?style=social) |
| [**Swift SDK**](https://github.com/absmartly/swift-sdk) | iOS and macOS SDK | ![Stars](https://img.shields.io/github/stars/absmartly/swift-sdk?style=social) |
| [**.NET SDK**](https://github.com/absmartly/dotnet-sdk) | C# and .NET SDK | ![Stars](https://img.shields.io/github/stars/absmartly/dotnet-sdk?style=social) |
| [**Vue2 SDK**](https://github.com/absmartly/vue2-sdk) | Vue 2 SDK with plugin support | ![Stars](https://img.shields.io/github/stars/absmartly/vue2-sdk?style=social) |

</div>

### Developer Tools

<div align="center">

| Tool | Description | Status |
|------|-------------|--------|
| [**Chrome Extension**](https://github.com/absmartly/absmartly-chrome-extension) | Visual experiment creation & debugging | 🚧 Beta |
| [**MCP Server**](https://github.com/absmartly/absmartly-mcp) | Model Context Protocol integration | ✅ Active |
| [**CLI Tools**](https://github.com/absmartly/cli) | Command-line interface for ABsmartly | ✅ Active |

</div>

## 🚀 Quick Start

### 1. Install an SDK

```bash
# JavaScript/TypeScript
npm install @absmartly/javascript-sdk

# Python
pip install absmartly

# Go
go get github.com/absmartly/go-sdk
```

### 2. Initialize the SDK

```javascript
import { ABsmartly } from '@absmartly/javascript-sdk';

const absmartly = new ABsmartly({
  endpoint: 'https://your-instance.absmartly.io/v1',
  apiKey: 'YOUR_API_KEY',
  application: 'your-app',
  environment: 'production'
});
```

### 3. Create an Experiment

```javascript
const context = absmartly.createContext({
  units: {
    userId: 'user-123',
    sessionId: 'session-456'
  }
});

const treatment = context.getTreatment('homepage-hero-test');
if (treatment === 1) {
  // Show variant A
} else {
  // Show variant B
}
```

## 📈 Why Choose ABsmartly?

### For Developers 👨‍💻
- **Type-safe SDKs** with excellent IDE support
- **Flexible targeting** with custom attributes
- **Webhook integrations** for CI/CD pipelines
- **REST API** for complete control

### For Product Teams 📊
- **Visual experiment builder** - no code required
- **Real-time analytics** with confidence intervals
- **Audience segmentation** and targeting
- **Collaborative workflows** with approval processes

### For Data Scientists 🔬
- **Bayesian statistics** for accurate decision-making
- **Sequential testing** to reduce sample sizes
- **Custom metrics** and goal tracking
- **Raw data exports** for advanced analysis

## 🤝 Contributing

We welcome contributions to all our open-source projects! Check out our [Contributing Guidelines](CONTRIBUTING.md) to get started.

### Ways to Contribute
- 🐛 Report bugs and issues
- 💡 Suggest new features
- 📖 Improve documentation
- 🔧 Submit pull requests

## 📚 Resources

- 📖 [Documentation](https://docs.absmartly.com) - Complete guides and API references
- 📝 [Blog](https://www.absmartly.com/blog) - Best practices and case studies
- 🎥 [Video Tutorials](https://www.youtube.com/@absmartly) - Step-by-step guides

## 🏢 About ABsmartly

ABsmartly is trusted by leading companies worldwide to power their experimentation programs. Our platform handles billions of events monthly, enabling teams to make confident, data-driven decisions.

<div align="center">
  <h3>Ready to accelerate your experimentation?</h3>
  
  [![Get Started](https://img.shields.io/badge/Get%20Started-Free%20Trial-success?style=for-the-badge&logo=rocket)](https://www.absmartly.com/signup)
  [![Contact Sales](https://img.shields.io/badge/Contact-Sales%20Team-blue?style=for-the-badge&logo=gmail)](https://www.absmartly.com/contact)
  [![Book Demo](https://img.shields.io/badge/Book-Live%20Demo-orange?style=for-the-badge&logo=calendar)](https://www.absmartly.com/demo)
</div>

---

<div align="center">
  <p>
    <a href="https://www.absmartly.com">Website</a> •
    <a href="https://docs.absmartly.com">Documentation</a> •
    <a href="https://www.absmartly.com/blog">Blog</a> •
    <a href="https://twitter.com/absmartly">Twitter</a> •
    <a href="https://www.linkedin.com/company/absmartly">LinkedIn</a>
  </p>
  
  <p>© 2024 ABsmartly. Built with ❤️ for developers and data teams.</p>
</div>