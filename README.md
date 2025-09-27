# 🎮 YouTube Playables Collection

A collection of playable games designed for the YouTube platform, featuring multiple game genres and styles.

## 🚀 Quick Start

### Local Development
```bash
# Install dependencies
npm install

# Start local server
npm run dev
```

Then open: http://localhost:8080

### Alternative Methods
```bash
# Python
python3 -m http.server 8080

# VS Code Live Server
# Install "Live Server" extension, then right-click index.html
```

## 🎯 Available Games

### 🪙 Coin Runner
- **Location**: `coin-runner/`
- **Type**: Endless Runner
- **Status**: ✅ Ready to Play
- **Features**: 
  - 3-lane running gameplay
  - Jump, slide, and lane switching
  - Coin collection system
  - Increasing difficulty
  - Touch and keyboard controls

### 🚀 Space Shooter
- **Location**: `space-shooter/`
- **Type**: Arcade Shooter
- **Status**: 🔄 In Development
- **Features**: (Coming Soon)

### 🧩 Puzzle Platformer
- **Location**: `puzzle-platformer/`
- **Type**: Puzzle Game
- **Status**: 📋 Planned
- **Features**: (Coming Soon)

### 🏎️ Racing Game
- **Location**: `racing-game/`
- **Type**: Racing
- **Status**: 📋 Planned
- **Features**: (Coming Soon)

## 🎮 Controls

### Coin Runner
- **Desktop**:
  - `A/D` or `←/→` - Switch lanes
  - `W` or `↑` or `Space` - Jump
  - `S` or `↓` - Slide
- **Mobile**:
  - Left side of screen - Move left
  - Right side of screen - Move right
  - Top center - Jump
  - Bottom center - Slide

## 🛠️ Development

### Project Structure
```
playables/
├── index.html              # Main menu
├── package.json            # Dependencies
├── README.md              # This file
├── coin-runner/           # Coin Runner game
│   └── index.html
├── space-shooter/         # Space Shooter game (planned)
├── puzzle-platformer/     # Puzzle game (planned)
└── racing-game/           # Racing game (planned)
```

### Adding New Games
1. Create new folder: `new-game/`
2. Add `index.html` with game code
3. Include YouTube Playables SDK
4. Implement required SDK functions
5. Add game card to main `index.html`

### YouTube Playables SDK Integration
Every game must include:
```html
<script src="https://www.youtube.com/game_api/v1"></script>
```

Required functions:
```javascript
// Notify when first frame is rendered
ytgame.game.firstFrameReady();

// Notify when game is ready
ytgame.game.gameReady();

// Handle audio settings
ytgame.system.isAudioEnabled();
ytgame.system.onAudioEnabledChange(callback);

// Handle pause/resume
ytgame.system.onPause(callback);
ytgame.system.onResume(callback);
```

## 🎨 Game Features

### Coin Runner Features
- **Endless Running**: Continuous gameplay with increasing speed
- **3-Lane System**: Switch between left, center, and right lanes
- **Jump & Slide**: Avoid obstacles by jumping or sliding
- **Coin Collection**: Collect coins for points
- **Progressive Difficulty**: Speed increases over time
- **Responsive Design**: Works on all screen sizes
- **Touch Controls**: Full mobile support
- **YouTube SDK**: Complete integration with YouTube Playables

## 🔧 Technical Details

### Technologies Used
- **HTML5 Canvas**: For game rendering
- **JavaScript**: Game logic and controls
- **CSS3**: Styling and responsive design
- **YouTube Playables SDK**: Platform integration

### Performance
- Optimized for 60 FPS gameplay
- Efficient collision detection
- Object pooling for obstacles and coins
- Responsive canvas sizing

### Browser Support
- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers

## 📱 Mobile Testing

### Testing on Mobile
1. Find your computer's IP address
2. Start local server: `npm run dev`
3. Open `http://YOUR_IP:8080` on mobile device
4. Test touch controls

### Mobile Features
- Touch controls for all games
- Responsive design
- Optimized performance
- Full-screen support

## 🚀 Deployment

### GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source branch (usually `main`)
4. Access via `https://yourusername.github.io/repository-name`

### Other Hosting
- Any static web hosting service
- CDN for better performance
- Custom domain support

## 📚 Resources

- [YouTube Playables Documentation](https://developers.google.com/youtube/gaming/playables)
- [HTML5 Canvas Tutorial](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [Game Development Best Practices](https://developer.mozilla.org/en-US/docs/Games)

## 🤝 Contributing

1. Fork the repository
2. Create feature branch: `git checkout -b feature/new-game`
3. Add your game to appropriate folder
4. Update main `index.html` with game card
5. Test thoroughly
6. Submit pull request

## 👨‍💻 Credits

**Created by:** Alg  
**GitHub:** [@anuplalgupta](https://github.com/anuplalgupta)  
**Project:** YouTube Playables Collection

### Special Thanks
- YouTube Playables team for the SDK and platform
- Open source community for inspiration and tools
- Contributors and testers

## 📄 License

MIT License - feel free to use this code for your own projects!

## 🎯 Roadmap

- [x] Coin Runner game
- [ ] Space Shooter game
- [ ] Puzzle Platformer game
- [ ] Racing game
- [ ] High score system
- [ ] Sound effects
- [ ] More game genres
- [ ] Multiplayer support

## 🐛 Bug Reports

Found a bug? Please create an issue with:
- Game name and version
- Steps to reproduce
- Expected vs actual behavior
- Browser and device information

## 💡 Feature Requests

Have an idea for a new game or feature? Create an issue and let's discuss!
