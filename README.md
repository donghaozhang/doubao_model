# Doubao Model Integration

A comprehensive Python project for integrating with Doubao (豆包) AI models, featuring both chat completion and video generation capabilities.

## 🚀 Features

- **Chat Completion**: Interactive AI conversations using Doubao's chat models
- **Video Generation**: Create videos from text prompts and images using Doubao's video generation API
- **Environment Security**: Secure API key management using environment variables
- **Web Interfaces**: Multiple HTML interfaces for testing and demonstration

## 📁 Project Structure

```
doubao_model/
├── doubao_chat_completion.py    # Chat completion functionality using OpenAI SDK
├── doubao_video_generation.py   # Video generation using Volcengine SDK
├── doubao_interface_v1.html     # Primary web interface for Doubao
├── doubao_interface_v2.html     # Enhanced web interface version
├── sample_webpage.html          # Sample webpage for testing
├── .env                         # Environment variables (API keys)
├── .gitignore                   # Git ignore rules
└── README.md                    # This file
```

## 🛠️ Setup

### Prerequisites

```bash
pip install openai python-dotenv
pip install 'volcengine-python-sdk[ark]'
```

### Environment Configuration

1. Create a `.env` file in the project root:
```bash
ARK_API_KEY=your_doubao_api_key_here
```

2. Replace `your_doubao_api_key_here` with your actual Doubao API key

## 🎯 Usage

### Chat Completion

```bash
python doubao_chat_completion.py
```

This script demonstrates:
- Image analysis capabilities
- Multi-modal input (text + image)
- Chinese language support

### Video Generation

```bash
python doubao_video_generation.py
```

This script demonstrates:
- Text-to-video generation
- Image-to-video generation
- Task polling and status monitoring
- High-resolution output (1080p)

## 🔧 Configuration

### API Endpoints

- **Base URL**: `https://ark.cn-beijing.volces.com/api/v3`
- **Chat Model**: `doubao-seed-1-6-thinking-250615`
- **Video Model**: `doubao-seedance-1-0-pro-250528`

### Video Generation Parameters

- **Resolution**: 1080p
- **Duration**: 5 seconds
- **Camera**: Dynamic (not fixed)

## 🌐 Web Interfaces

- **doubao_interface_v1.html**: Primary interface for Doubao interactions
- **doubao_interface_v2.html**: Enhanced version with additional features
- **sample_webpage.html**: Testing and demonstration webpage

## 🔒 Security

- API keys are stored in environment variables
- `.env` file is excluded from version control
- No sensitive information in source code

## 📝 API Documentation

For more detailed API usage:
- [Video Generation Tasks](https://www.volcengine.com/docs/82379/1521675)
- [Task Management](https://www.volcengine.com/docs/82379/1521720)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is open source and available under the MIT License.

## ⚠️ Important Notes

- Ensure your API key has appropriate permissions
- Monitor usage to avoid exceeding rate limits
- Video generation may take several minutes to complete
- Keep your `.env` file secure and never commit it to version control 