# San Jose Map Poster Generator

Generate beautiful minimalist map posters of San Jose, California with a tech-inspired dark + cyan aesthetic that honors Silicon Valley's identity.

## Design

**Tech Minimalist Theme:**
- Deep navy background (#0d1b2a)
- Cyan road network (#00d4ff)
- Teal water features (#1b4965)
- Muted sage parks (#1e3a2f)
- Clean typography

The design echoes the circuit-board aesthetic of Silicon Valley while creating a striking, frameable piece of art.

## Installation

```bash
# Clone the repo
git clone https://github.com/neildharrington/sanjose-map-poster.git
cd sanjose-map-poster

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Usage

```bash
# Generate default San Jose poster
python generate_poster.py

# Custom radius (in km)
python generate_poster.py --radius 20

# Custom output filename
python generate_poster.py --output my_poster.png

# High resolution (300 DPI)
python generate_poster.py --dpi 300
```

## Options

| Argument | Default | Description |
|----------|---------|-------------|
| `--radius` | 25 | Radius in kilometers from city center |
| `--output` | `sanjose_poster.png` | Output filename |
| `--dpi` | 150 | Resolution (use 300 for print quality) |
| `--no-labels` | False | Omit city name text |

## Output

Generates a high-quality PNG suitable for:
- 18x24" poster prints
- Digital wallpapers
- Framed artwork

## Tech Stack

- **OSMnx** - OpenStreetMap data retrieval
- **Matplotlib** - Rendering
- **Shapely** - Geometry handling
- **GeoPandas** - Geographic data processing

## License

MIT
