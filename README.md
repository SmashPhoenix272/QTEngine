# QTEngine: Chinese to Sino-Vietnamese Translation Engine

## Overview
QTEngine is an engine designed to convert Chinese text to Sino-Vietnamese.

## Features
- Advanced text processing for Chinese to Sino-Vietnamese translation
- Modular architecture with separate components for:
  - Character utilities
  - Text processing
  - Data loading
  - Performance profiling
- Trie-based data structure for efficient text manipulation
- Logging and performance tracking

## Project Structure
```
QTEngine/
│
├── src/                    # Core source code modules
│   ├── character_utils.py  # Character-level utility functions
│   ├── data_loader.py      # Data loading and management
│   ├── data_watcher.py     # File and data monitoring
│   ├── performance.py      # Performance profiling tools
│   ├── text_processing.py  # Text processing and transformation
│   └── translation_engine.py  # Base translation engine
│
├── models/                 # Data structures and models
│   └── trie.py             # Trie data structure implementation
│
├── data/                   # Data files and resources
├── tests/                  # Unit and integration tests
├── translated_result/      # Output directory for translated texts
│
├── QTEngine.py             # Main translation engine class
├── config.py               # Configuration settings
└── requirements.txt        # Project dependencies
```

Data Files (Not included in repository)
The engine requires several data files for translation and text processing:

ChinesePhienAmWords.txt: Chinese to Sino-Vietnamese word mappings
Names.txt: Name translations
VietPhrase.txt: Vietnamese phrases and translations
These files should be placed in a data directory 

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/QTEngine.git
cd QTEngine
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
```python
from QTEngine import QTEngine

# Initialize the translation engine
engine = QTEngine()

# Translate Chinese text to Sino-Vietnamese
chinese_text = "你好，世界"
translated_text = engine.translate(chinese_text)
print(translated_text)
```

## Dependencies
- Python 3.7+
- watchdog (3.0.0)

## Key Components
- **Text Processing**: Advanced algorithms for converting Chinese text
- **Data Loader**: Efficient data management and loading
- **Performance Tracking**: Built-in profiling for translation operations
- **Trie Data Structure**: Optimized text manipulation

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
