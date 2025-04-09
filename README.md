# 🌙 Tokyo Night Tmux Configuration

A professional, minimal, and highly functional tmux configuration with Tokyo Night theme integration, Vim-like keybindings, and productivity enhancements.

## ✨ Features

- **🎨 Tokyo Night Theme** - Stylish and easy-on-the-eyes color scheme
- **🖥️ True Color Support** - 24-bit color compatibility
- **🐭 Mouse Integration** - Full mouse support for pane/window management
- **📋 System Clipboard** - Seamless integration with OS clipboard
- **⏳ Session Persistence** - Auto-save/restore sessions with `tmux-resurrect`
- **🔌 Plugin Ecosystem** - Extended functionality through curated plugins
- **⌨️ Vim-style Navigation** - Intuitive keybindings for Vim users
- **⚡ Performance Optimized** - Fast response times and smooth operation

## 🚀 Installation

### Requirements
- Git 2.4.11+
- tmux 3.2+
- Terminal with True Color support (WezTerm, iTerm2, Kitty, etc.)

### Quick Start
```bash
# Clone the repository
git clone https://github.com/yourusername/tokyo-night-tmux.git ~/.config/tmux

# Create symlink to tmux config
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf

# Install TPM (Tmux Plugin Manager)
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Start tmux and install plugins
tmux new -s tmp
# Inside tmux, press: Ctrl-Space + Shift-I
```

## ⌨️ Key Bindings

### Session Management
| Binding         | Action                          |
|-----------------|---------------------------------|
| `Ctrl-Space S`  | Create new session              |
| `Ctrl-Space B`  | Choose session from list        |
| `Ctrl-Space D`  | Detach from session             |

### Window Management
| Binding         | Action                          |
|-----------------|---------------------------------|
| `Ctrl-Space C`  | Create new window               |
| `Ctrl-Space M-c`| Close current window            |
| `Ctrl-Space N`  | Next window                     |
| `Ctrl-Space P`  | Previous window                 |

### Pane Management
| Binding         | Action                          |
|-----------------|---------------------------------|
| `Ctrl-Space %`  | Split vertically                |
| `Ctrl-Space "`  | Split horizontally              |
| `Ctrl-Space Z`  | Toggle pane zoom                |
| `Ctrl-Space X`  | Close current pane              |

### Navigation
| Binding         | Action                          |
|-----------------|---------------------------------|
| `Ctrl-Space H`  | Move left (Vim style)           |
| `Ctrl-Space J`  | Move down (Vim style)           |
| `Ctrl-Space K`  | Move up (Vim style)             |
| `Ctrl-Space L`  | Move right (Vim style)          |
| `Alt-Arrow`     | Move between panes (no prefix)  |

## 🔌 Plugins Included

- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) - Session persistence
- [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) - Auto-save sessions
- [tmux-fzf](https://github.com/sainnhe/tmux-fzf) - Fuzzy finder integration
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) - Seamless Vim navigation
- [tmux-yank](https://github.com/tmux-plugins/tmux-yank) - System clipboard integration

## 🎨 Customization

### Change Theme Flavor
```tmux
# In ~/.tmux.conf
set -g @tokyo-night-tmux_theme 'night'  # Available: night, storm
```

### Modify Status Bar
```tmux
# Show/hide battery status
set -g @tokyo-night-tmux_show_battery 0

# Change date format
set -g @tokyo-night-tmux_date_format '%Y-%m-%d'
```

## 🛠️ Troubleshooting

**Q: Colors look wrong in my terminal**  
```bash
# Verify truecolor support
curl -s https://gist.githubusercontent.com/lifepillar/09a44b8cf0f9397465614e622979107f/raw/24-bit-color.sh | bash
```

**Q: Prefix key not working**  
```bash
# Check for conflicting applications
# Try changing escape-time in config:
set -sg escape-time 50
```

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first.

## 📄 License
[MIT](https://choosealicense.com/licenses/mit/)

---

**Maintained with ❤️ by [Dev Kraken]**  
[![GitHub Stars](https://img.shields.io/github/stars/dev-kraken/tmux?style=social)](https://github.com/dev-kraken/tmux)
[![tmux](https://img.shields.io/badge/tmux-3.2+-blue.svg)](https://github.com/tmux/tmux)
