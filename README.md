# BPCC KT Tracker

A professional Knowledge Transfer (KT) tracking system for BITS Pilani Consulting Club, designed to help members stay informed about upcoming training sessions and workshops.

## Features

- **Interactive Calendar** - Visual month view with KT indicators on scheduled dates
- **Live Countdown** - Real-time countdown to the next KT session
- **Session Details** - Comprehensive information including presenter, venue, agenda, and relevance
- **Month Navigation** - Browse current and next month's KT sessions
- **Responsive Design** - Clean, professional interface with smooth interactions
- **Dynamic Data** - Easy-to-update JSON-based KT schedule

## Tech Stack

- **HTML5** - Semantic structure
- **CSS3** - Custom styling with Tailwind CSS utility classes
- **Vanilla JavaScript** - No dependencies, pure JS implementation
- **JSON** - Centralized data management

## Project Structure

```
kt-tracker/
├── index.html          # Main HTML file
├── main.css            # Custom styles and animations
├── ktdata.json         # KT schedule data
├── photos/
│   └── bpcclogo_light.png
└── README.md
```

## Quick Start

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd kt-tracker
   ```

2. **Start a local server**

   ```bash
   # Using Python
   python -m http.server 3000

   # Using Node.js
   npx http-server -p 3000
   ```

3. **Open in browser**
   ```
   http://localhost:3000
   ```

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Import project in Vercel
3. Deploy - no configuration needed (uses `vercel.json`)

The site will be live at `https://your-project.vercel.app`

## Managing KT Data

Edit `ktdata.json` to add, update, or remove KT sessions:

```json
{
  "topic": "Session Title",
  "presenter": "Presenter Name",
  "date": "2025-11-14T00:00:00",
  "time": "TBA",
  "venue": "Venue Name",
  "agenda": ["Topic 1", "Topic 2"],
  "relevance": "Why this session matters"
}
```

**Time Field:**

- Specific time: `"10:00 PM"`
- To be announced: `"TBA"` (countdown uses 12:00 AM of that date)

## Features in Detail

### Calendar View

- Current day highlighted in blue
- KT dates marked with blue indicator dots
- Click any KT date to view full session details
- Navigate between current and next month only

### Next KT Widget

- Shows upcoming session at the top
- Live countdown timer (updates every second)
- Quick overview of date, time, venue, and presenter

### Session Modal

- Professional card-based layout
- Scrollable content for longer agendas
- Presenter, date/time, venue, agenda, and relevance sections
- Responsive design that fits within viewport

## Design Philosophy

- **Professional & Clean** - No gimmicky animations, static and elegant
- **Blue & White Theme** - Consistent color scheme throughout
- **Accessibility** - Clear typography and intuitive navigation
- **Performance** - Lightweight with no external dependencies

## Browser Support

Works on all modern browsers:

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## Contributing

To add new KT sessions:

1. Edit `ktdata.json`
2. Follow the existing JSON structure
3. Refresh the page to see changes

## License

Private project for BITS Pilani Consulting Club

---

**Made with ❤️ for BPCC**
