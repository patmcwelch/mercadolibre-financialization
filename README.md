# MercadoLibre Financialization Visualization

An interactive, scroll-based data visualization telling the story of MercadoLibre's dramatic transformation from Latin America's largest e-commerce platform into a financial services powerhouse.

## Overview

Between 2018 and 2025, MercadoLibre underwent a fundamental business shift—financialization. Financial services revenue grew from just 17% to 43% of total revenue, driven primarily by Brazil's high interest rate environment (SELIC reaching 15% in 2025). This visualization tells that story through five animated sections revealing:

- **Revenue evolution**: How fintech grew from $300M to $11.2B
- **Brazil context**: The correlation between SELIC rates and fintech profitability
- **Margin comparison**: Why financial services (42% margin) beat commerce (28% margin)
- **Key insights**: 30x credit portfolio growth and the complete transformation

## Features

- **Single self-contained HTML file** - No dependencies, no build process
- **Scroll-triggered animations** - Each section reveals as you scroll
- **Pure vanilla JavaScript** - No frameworks or libraries
- **Hand-coded SVG charts** - Stacked area, dual-axis line, radial progress
- **Fully responsive** - Adapts to desktop, tablet, and mobile
- **Dark theme** - Brazil-inspired color palette (green/yellow accents)

## Usage

Simply open `index.html` in any modern web browser:

```bash
open index.html
```

Or view the live demo: [MercadoLibre Financialization](https://mcwelch.com/mercadolibre-financialization/)

## Technical Details

### Architecture

- **Single file design**: All CSS, JavaScript, and data embedded in one HTML file
- **Intersection Observer API**: Triggers animations at 30% viewport threshold
- **SVG animations**: Stroke-dasharray technique for path drawing
- **Custom easing**: easeOutCubic function for smooth number counters
- **Responsive grid**: CSS Grid and Flexbox for adaptive layouts

### Performance

- **60fps animations**: Using requestAnimationFrame for smooth counters
- **Progressive enhancement**: Works without JavaScript (static display)
- **Optimized SVG**: Hand-coded paths, no external charting libraries
- **Google Fonts**: Inter font family (only external dependency)

### Data Sources

All financial data based on MercadoLibre investor reports and public filings:

- Revenue data (2018-2025): Commerce vs Fintech breakdown
- Brazil SELIC rates: Central Bank of Brazil official rates
- Profit margins: Segment operating margins from quarterly reports
- Credit portfolio: Total credit book value growth

## Structure

### Sections

1. **Hero** (100vh) - Animated 17% → 43% counter
2. **Revenue Evolution** (70vh) - Stacked area chart
3. **Brazil Context** (80vh) - Dual-axis line chart with context panel
4. **Margin Comparison** (60vh) - Radial progress indicators
5. **Key Insights** (50vh) - Three stat cards with conclusion

## Design System

### Color Palette

```css
--bg-dark: #0a0a0a           /* Background */
--card-bg: #141414           /* Card backgrounds */
--fintech-green: #10b981     /* Financial services data */
--commerce-blue: #3b82f6     /* Commerce data */
--selic-red: #ef4444         /* Interest rate data */
--brazil-green: #009b3a      /* Brazil accent */
--brazil-yellow: #fedf00     /* Brazil accent */
```

### Typography

- **Font**: Inter (Google Fonts)
- **Hero title**: 4rem bold
- **Section titles**: 2rem semibold
- **Body text**: 1rem regular
- **Labels**: 0.75rem uppercase

### Responsive Breakpoints

- **Desktop**: 1200px+ (full layout)
- **Tablet**: 768px - 1199px (adapted grid)
- **Mobile**: < 768px (single column stack)

## Browser Support

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Opera 74+

Requires support for:
- CSS Grid & Flexbox
- SVG 1.1
- Intersection Observer API
- CSS Custom Properties

## License

MIT License - Free to use and modify

## Credits

- **Data visualization**: Custom SVG charts with scroll animations
- **Typography**: Inter font family by Rasmus Andersson
- **AI assistance**: Claude Sonnet 4.5
