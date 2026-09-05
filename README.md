# Suger Cane Client

A high-performance Minecraft 1.13 client built with optimized WebAssembly (WASM) technology.

## Overview

Suger Cane is a next-generation Minecraft client that improves upon the traditional 1.13 WASM experience through careful optimization and performance enhancements. This client prioritizes **smooth gameplay** and **efficient resource usage** while maintaining full compatibility with 1.13 server features.

## Key Features

✨ **Performance-Optimized**
- Utilizes advanced WebGL2 rendering with fallback to WebGL for broader compatibility
- Intelligent device pixel ratio scaling (capped at 1.5x) to maintain high FPS on high-DPI displays
- Streamlined rendering pipeline that minimizes unnecessary GPU operations

⚡ **Efficient Rendering**
- High-performance graphics context with:
  - Alpha blending disabled for faster compositing
  - Antialiasing disabled to reduce GPU overhead
  - Power preference set to high-performance mode
  - Drawing buffer optimization for faster frame rates

🎮 **Responsive Controls**
- Server connection with real-time WebSocket (WSS) support
- Frame-timing synchronized with `requestAnimationFrame` for buttery-smooth 60+ FPS
- Real-time FPS monitoring for performance tracking

🖥️ **Cross-Platform**
- Runs in any modern web browser
- Responsive canvas that adapts to window resizing
- Mobile-friendly viewport settings for on-the-go gameplay

## Technical Highlights

### Optimization Advantages Over Standard 1.13 WASM

This client implements several key optimizations:

1. **Rendering Efficiency** - Only essential buffer clears, reducing GPU stalls
2. **Resolution Scaling** - Dynamic device pixel ratio capping prevents performance cliffs on ultra-high-DPI displays
3. **WebGL2 Priority** - Takes advantage of WebGL2's superior performance and features where available
4. **Memory Management** - Optimized context parameters reduce memory footprint and GPU bandwidth usage

## Getting Started

1. Open the `Sugercane-client-V0.html` file in your browser
2. Enter your server address (default: `wss://arch.mc`)
3. Connect and start playing!

## Server Configuration

To connect to a different server, modify the server input field in the client UI or update the default value in the HTML:

```html
<input id="server" type="text" value="wss://your-server.com" />
```

## Development Status

🚧 **Work in Progress** - This project is actively being developed. Features and optimizations are continually being refined.

## System Requirements

- Modern web browser with WebGL/WebGL2 support (Chrome, Firefox, Safari, Edge)
- Minimum 100MB free RAM
- Stable internet connection for server communication

---

**Built with performance in mind.** Suger Cane brings optimized 1.13 gameplay to the web.
