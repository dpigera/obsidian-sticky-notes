# Obsidian Sticky Notes Plugin

A plugin for [Obsidian](https://obsidian.md) that allows you to create notes inline without moving your cursor.

## Features

- Type 'Sticky' to quickly use Command palette command
- Specify a default folder for saving your sticky notes
- Press Enter to save the note as a new file in your vault
- Press Escape to cancel and close the sticky note
- Automatically returns focus to your document after saving or closing a sticky note

## Screenshots
![Demo](https://tilt-vc-static.s3.us-east-1.amazonaws.com/obsidian-stickynote-github-pics/obsidian-demo.gif)

## Installation

### From Obsidian Community Plugins

1. Open Obsidian
2. Go to Settings > Community plugins
3. Click "Browse" and search for "Sticky Notes"
4. Install the plugin and enable it

### Manual Installation

1. Download the latest release from the [GitHub repository](https://github.com/dpigera/obsidian-postit-extension/releases)
2. Extract the zip file into your Obsidian vault's `.obsidian/plugins/` directory
3. Reload Obsidian
4. Enable the plugin in Settings > Community plugins

## Usage

1. Use the command palette (Ctrl/Cmd+P) and search for "Create Sticky Note"
2. Type your note content in the yellow sticky note
3. Press Enter to save as a new note, or Escape to cancel

## Settings

- **Default Folder**: Specify a folder path where sticky notes will be saved. Use "/" for the root folder.

## How It Works

- The sticky note appears at the left side of your document at the same vertical position as your cursor
- Only one sticky note can exist at a time
- When you save a note, it creates a new markdown file in your specified default folder
- The title of the note is derived from the first 15 characters of your content
- After saving or closing a note, focus returns to your document at the same position

## Development

This plugin uses JavaScript and follows the Obsidian plugin development guidelines.

### Project Structure

- `main.dev.js`: The source file for development
- `main.js`: The bundled output file (generated by esbuild)
- `styles.css`: CSS styles for the plugin
- `manifest.json`: Plugin metadata

### Building

1. Clone this repository
2. Run `npm install` to install dependencies
3. Make changes to `main.dev.js` (not `main.js`)
4. Run `npm run build` to compile the plugin

## Support

If you find this plugin useful, consider supporting its development:

[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="BuyMeACoffee" width="200">](https://www.buymeacoffee.com/yourusername)

## License

[MIT](LICENSE) 
