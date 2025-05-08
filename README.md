# Made as part of Live Coding Olympics
[![Watch the video](https://img.youtube.com/vi/xySgNhHz4PI/0.jpg)](https://youtu.be/xySgNhHz4PI)

Full results with links:
https://docs.google.com/spreadsheets/d/1kgnVU6NZVTwqtUkrNetXTpm0oY7NsYGJn61u6-JMIoI/edit?usp=sharing

# OpenAI Image Models Comparison Tool - Made with [Desktop Commander](https://desktopcommander.app/) and Claude Desktop for Vibe Coding comparison

A web-based tool to compare image generation across OpenAI's DALL-E 2, DALL-E 3, and GPT Image-1 (newest) models side-by-side.

## Features

- 🎨 **Parallel Image Generation**: Generate images with all three models simultaneously
- 🔄 **Real-time Comparison**: See the differences between model generations
- ⏱️ **Performance Metrics**: Track generation time for each model
- 🔐 **Secure API Key Storage**: Local storage for API credentials
- 📱 **Responsive Design**: Works on desktop and mobile devices
- 💡 **Revised Prompts**: View DALL-E 3's prompt revisions

## Live Demo

Visit the [live demo](https://wonderwhy-er.github.io/openai-image-compare-claudedesktop/) on GitHub Pages.

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/openai-image-compare-claudedesktop.git
   ```

2. Open `index.html` in your browser or serve it locally:
   ```bash
   cd openai-image-compare-claudedesktop
   python -m http.server 8000
   # Visit http://localhost:8000
   ```

3. Enter your OpenAI API key and start generating images!

## Usage

1. **Enter API Key**: Your OpenAI API key is required to use this tool. It's stored locally in your browser.
2. **Write Prompt**: Enter a descriptive prompt for image generation.
3. **Generate**: Click the "Generate Images" button to create images with all three models.
4. **Compare**: View the results side-by-side to compare quality and style.

## Technical Details

### Supported Models

- **DALL-E 2**: The original OpenAI image generation model
- **DALL-E 3**: Improved model with better prompt adherence
- **GPT Image-1**: The latest model with advanced capabilities

### API Integration

The tool uses the OpenAI Images API with the following specifications:

- **Endpoint**: `https://api.openai.com/v1/images/generations`
- **Image Size**: 1024x1024 pixels
- **Quality**: HD for DALL-E 3 (when supported)
- **Response Format**: URL for DALL-E 2/3, base64 for GPT Image-1

## Project Structure

```
openai-image-compare-claudedesktop/
├── index.html      # Main application file
└── README.md       # Project documentation
```

## Publishing to GitHub Pages

1. Create a new repository on GitHub
2. Push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/your-username/openai-image-compare-claudedesktop.git
   git push -u origin main
   ```
3. Enable GitHub Pages:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click Save

Your site will be available at: `https://your-username.github.io/openai-image-compare-claudedesktop/`

## Security Notes

- API keys are stored in browser localStorage
- Never commit API keys to version control
- Consider using environment variables in production

## Troubleshooting

### Common Issues

1. **"Invalid API key" error**: Check that your API key is correct and has image generation permissions
2. **Empty images**: GPT Image-1 returns base64 data, ensure your browser supports data URIs
3. **CORS issues**: If running locally, use a local server (e.g., `python -m http.server`)

### Error Messages

- **401 Unauthorized**: Invalid API key
- **429 Too Many Requests**: Rate limit exceeded, wait before retrying
- **400 Bad Request**: Check prompt format and model parameters

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - feel free to use this project for your own purposes.

## Acknowledgments

- Built for comparing OpenAI's image generation models
- Inspired by the rapid evolution of AI image generation

## Contact

For questions or feedback, please open an issue on GitHub.

---

Made with ❤️ using OpenAI's image generation APIs
