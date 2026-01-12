# 🏈 4th Down Decision Tool

A data-driven web application that helps football coaches make optimal decisions on 4th down situations. Built with modern analytics principles and an intuitive user interface.

## Features

### Game Situation Inputs
- **Field Position** - Interactive slider showing position on visual field diagram
- **Yards to Go** - First down distance (1-15+ yards)
- **Score** - Current game score for both teams
- **Quarter & Time** - Full game clock tracking
- **Timeouts** - Both team's remaining timeouts

### Team & Situational Factors
- **Offensive Strength** - Your team's short-yardage conversion ability
- **Defensive Strength** - Opponent's defensive quality
- **Kicker Accuracy** - Field goal success probability adjustment
- **Punter Quality** - Expected punt distance and placement
- **Weather Conditions** - Clear, windy, rain, or snow impacts
- **Game Context** - Regular season, rivalry, playoff, or championship
- **Momentum** - Current game momentum indicator

### Decision Analytics
- **Three Options Compared**: Go For It, Punt, or Field Goal
- **Expected Points Added (EPA)** - Statistical value of each decision
- **Conversion Probability** - Based on yards to go and team factors
- **Field Goal Success Rate** - Distance and weather adjusted
- **Win Probability Impact** - How each choice affects winning

### Smart Factors Analysis
The tool explains key factors influencing the recommendation:
- Field position advantages/risks
- Short vs. long yardage situations
- Time pressure and score differential
- Weather impacts on kicking game
- Team strength matchups

## Quick Scenarios

Pre-loaded scenarios for common situations:
- **4th & Short (Goal Line)** - Red zone decision
- **4th & 3 (Midfield)** - Classic go/punt dilemma
- **Trailing Late (2-min)** - Desperate comeback situation
- **FG Range Decision** - Kick vs. go for more points
- **Own Territory** - Risk vs. reward deep in your own end

## How to Use

1. **Open `index.html`** in any modern web browser
2. **Set the game situation** using the sliders and inputs
3. **Adjust team factors** to match your teams' strengths
4. **Click "Calculate Recommendation"** or adjustments auto-calculate
5. **Review the analysis** including factors and probability breakdown

## The Algorithm

The decision engine uses expected value calculations based on:

### Conversion Rates
Based on NFL historical data by yards to go:
- 4th & 1: ~72% conversion rate
- 4th & 3: ~54% conversion rate
- 4th & 5: ~44% conversion rate
- 4th & 10: ~29% conversion rate

### Expected Points Model
Field position-based expected points:
- Opponent's 5 yard line: ~5.0 EP
- Opponent's 20: ~2.9 EP
- Midfield: ~0.5 EP
- Own 20: ~-0.7 EP

### Adjustments Applied
- Offensive/defensive strength modifiers
- Weather impacts (more significant for kicking)
- Time pressure multipliers (aggressive when trailing late)
- Game context (higher stakes = more aggressive)
- Momentum factors

## Browser Support

Works in all modern browsers:
- Chrome (recommended)
- Firefox
- Safari
- Edge

## Local Development

Simply open `index.html` in a browser. No build process or dependencies required.

For local server (optional):
```bash
python -m http.server 8000
# Then visit http://localhost:8000
```

## Credits

Built with modern web technologies:
- Pure HTML5, CSS3, and JavaScript
- Inter font family from Google Fonts
- Responsive design for all screen sizes

Analytics model inspired by NFL Next Gen Stats and academic research on 4th down decision-making.

---

*Note: This tool provides data-driven recommendations but should be used alongside coaching judgment and team-specific knowledge. Always consider your unique team dynamics and game situation.*
