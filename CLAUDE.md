# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Japanese font text trim visualization tool - a simple static web application that compares vertical text alignment across different fonts. The project helps visualize how Japanese and English fonts handle vertical spacing differently, particularly useful for UI design considerations.

## Architecture

- **Static HTML/CSS/JS**: No build process or dependencies required
- **Single page application**: All functionality contained in `index.html`
- **Font comparison focus**: Compares Hiragino Kaku Gothic (Japanese), Noto Sans JP (Japanese), and Roboto (English)
- **Visualization approach**: Uses center lines and visual containers to show font baseline differences

## Key Components

- `index.html`: Main application with button comparison sections and text sample visualization
- `app.css`: Complete styling including responsive design, font-specific classes, and visualization containers
- Button sections display fonts with/without center lines for comparison
- Text sample section shows mixed Japanese/English characters with visual bounding boxes

## Development

**Running the application:**
- Open `index.html` directly in a web browser (no server required)
- All dependencies loaded via CDN (Google Fonts)

**Font classes:**
- `.hiragino-button`: Uses Hiragino Kaku Gothic Pro font family
- `.english-button`: Uses Roboto font family  
- Default buttons use Noto Sans JP
- `.no-line` class removes center alignment line

**Responsive breakpoints:**
- 768px: Tablet layout adjustments
- 480px: Mobile layout with reduced font sizes and padding

## CSS Architecture

The styling uses CSS Grid and Flexbox for layout, with a focus on:
- Button comparison sections with consistent sizing (60px height)
- Visual alignment indicators via CSS pseudo-elements
- Typography-focused design with emphasis on font rendering differences
- Mobile-first responsive approach