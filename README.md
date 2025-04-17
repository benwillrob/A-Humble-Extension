# Humble AI Chat Assistant

A Chrome extension that provides seamless access to Humble AI's powerful language models directly from your browser.

![Humble AI Chat Assistant](https://static.wixstatic.com/media/220c91_447a86e352ef456f8682a4afe3a83852~mv2.png/v1/fit/w_2500,h_1330,al_c/220c91_447a86e352ef456f8682a4afe3a83852~mv2.png)

## Overview

Humble AI Chat Assistant is a Chrome extension that allows you to interact with Humble AI's language models without leaving your browser. It provides a clean, intuitive interface for sending queries and receiving responses, with support for multiple BASE IDs, context-aware conversations, and theme customization.

## Features

- **Instant Access**: Chat with Humble AI directly from your browser with a simple keyboard shortcut
- **Context Menu Integration**: Select text on any webpage and right-click to "Ask Humble" about it
- **Multiple BASE IDs**: Configure and switch between different Humble AI BASE IDs
- **Context-Aware Conversations**: Maintain conversation context for more relevant responses
- **Theme Support**: Choose between light and dark themes
- **Markdown Formatting**: Support for bold text formatting in responses
- **Debug Mode**: Advanced debugging tools for troubleshooting
- **Responsive Design**: Clean, intuitive interface that works across different screen sizes

## How It Works

### Technical Architecture

The extension consists of several key components:

1. **Popup Interface**: The main chat interface that appears when you click the extension icon or use the keyboard shortcut
2. **Background Service Worker**: Handles context menu integration and maintains extension state
3. **Options Page**: Allows configuration of API keys, BASE IDs, and other settings
4. **API Integration**: Communicates with the Humble AI API to create chats and exchange messages

### Data Flow

1. When you open the extension, it checks for an existing chat session or creates a new one
2. Your messages are sent to the Humble AI API using your configured API key and BASE ID
3. Responses are processed and displayed in the chat interface
4. Chat history is stored locally in your browser for continuity between sessions

### API Integration

The extension communicates with the Humble AI platform through several API endpoints:

- Creating new chats
- Sending messages to existing chats
- Fetching available contexts for BASE IDs
- Submitting direct queries

## Installation

1. Download the extension files or clone this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" in the top-right corner
4. Click "Load unpacked" and select the extension directory
5. The Humble AI Chat Assistant icon will appear in your browser toolbar

## Configuration

Before using the extension, you'll need to configure it with your Humble AI credentials:

1. Click the extension icon and then click the settings icon (⚙️)
2. Enter your Humble AI API key
3. Add at least one BASE ID with a descriptive name
4. Set your preferred BASE ID as the default
5. Save your settings

## Usage

### Starting a Conversation

1. Click the extension icon in your browser toolbar or use the keyboard shortcut (Ctrl+Shift+Space or Cmd+Shift+Space on Mac)
2. Select a BASE ID from the dropdown menu
3. Type your message in the input field and press Enter or click the send button

### Using the Context Menu

1. Select text on any webpage
2. Right-click and select "Ask Humble about [selected text]"
3. The extension popup will open with the selected text pre-filled

### Switching BASE IDs

1. Open the extension popup
2. Select a different BASE ID from the dropdown menu
3. Your input will be preserved when switching between BASE IDs

### Clearing Chat History

1. Open the extension popup
2. Click "Clear Chat" at the bottom of the interface

## Advanced Features

### Debug Mode

1. Right-click the extension icon in your browser toolbar
2. Select "Toggle Debug Mode"
3. When enabled, the debug panel can be accessed from the extension popup

### Exporting Logs

1. Open the extension options page
2. Scroll to the "Debug & Troubleshooting" section
3. Click "Export Debug Logs"

## Privacy & Security

- All communication with the Humble AI API is secured using HTTPS
- Your API key is stored securely in Chrome's extension storage
- Chat history is stored locally in your browser and is not shared with third parties


## Acknowledgements

- Icons provided by [Lucide](https://lucide.dev/)
- UI components inspired by [shadcn/ui](https://ui.shadcn.com/)
