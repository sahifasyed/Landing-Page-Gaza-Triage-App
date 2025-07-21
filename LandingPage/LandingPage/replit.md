# Gaza Triage App

## Overview

This is an offline emergency triage application specifically designed for Gaza. The application focuses on providing life-saving medical triage capabilities that work without internet connectivity. It's a single-page HTML application with embedded CSS and appears to be designed for emergency medical situations where internet access may be unreliable or unavailable.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Technology**: Pure HTML5 with embedded CSS
- **Design Pattern**: Single-page application (SPA) approach
- **Styling**: CSS3 with custom properties (CSS variables) for theming
- **Responsive Design**: Mobile-first approach with viewport meta tag
- **Offline Capability**: Self-contained HTML file that can work without internet

### Key Design Decisions
- **Offline-First**: Everything is embedded in a single HTML file to ensure the app works in areas with poor or no internet connectivity
- **Accessibility**: Supports both LTR and RTL text direction for Arabic/English language support
- **Emergency-Focused UI**: Uses emergency color schemes (red for urgent situations) and medical-appropriate styling

## Key Components

### Visual Design System
- **Color Palette**: 
  - Primary: Dark blue (#1B2A41)
  - Accent: Medium blue (#3A506B) 
  - Emergency: Red (#D64545)
  - Background: Light gray (#F4F6F8)
- **Typography**: System fonts for reliability and fast loading
- **Animations**: Background animations for visual appeal
- **Shadows**: Soft shadows for depth and modern UI feel

### Internationalization
- **RTL/LTR Support**: Built-in support for both right-to-left (Arabic) and left-to-right (English) text directions
- **Language Switching**: Prepared for multilingual support

### Responsive Design
- **Mobile-First**: Designed primarily for mobile devices (likely tablets/phones used in medical settings)
- **Viewport Optimization**: Properly configured for mobile displays

## Data Flow

### Current State
- **Static Application**: Currently appears to be a static HTML file
- **No Backend**: No server-side components identified
- **Local Storage**: Likely uses browser localStorage for offline data persistence (implementation not visible in provided files)

### Expected Data Flow
- User inputs patient information
- Triage algorithm processes symptoms/vitals
- Results stored locally in browser
- Data persists offline for later synchronization when internet becomes available

## External Dependencies

### Minimal Dependencies
- **Fonts**: System fonts only (no external font loading)
- **Icons**: Inline SVG for favicon (no external icon libraries)
- **No CDN Dependencies**: Everything self-contained for offline reliability

### Rationale
- **Offline Reliability**: No external dependencies ensure the app works in internet-limited environments
- **Fast Loading**: Embedded resources eliminate network requests
- **Emergency Readiness**: Critical for emergency medical situations where connectivity is unreliable

## Deployment Strategy

### Current Deployment
- **Static File**: Single HTML file that can be served from any web server
- **Local Access**: Can be opened directly in browser from file system
- **Portable**: Easy to distribute via USB drives, messaging apps, or simple file sharing

### Recommended Deployment Options
1. **Static Hosting**: GitHub Pages, Netlify, or similar static hosting services
2. **Local Networks**: Can be hosted on local hospital/clinic networks
3. **Offline Distribution**: USB drives or local file sharing for areas without internet
4. **Progressive Web App**: Could be enhanced to work as a PWA for app-like experience

### Scalability Considerations
- **Stateless**: No server-side state management needed
- **CDN Ready**: Single file can be easily distributed via CDN
- **Version Control**: Simple file updates for new versions
- **Caching**: Entire app can be cached for offline use

## Development Notes

### Current State
The application appears to be in early development stages with:
- Basic HTML structure established
- CSS design system implemented
- Offline-first architecture planned
- Internationalization groundwork laid

### Missing Components (Likely to be Added)
- JavaScript functionality for triage logic
- Patient data input forms
- Triage algorithm implementation
- Local storage management
- Print functionality for patient records
- Data export capabilities

### Security Considerations
- **No Server**: Eliminates many server-side security concerns
- **Local Data**: Patient data stays on device (important for privacy)
- **HTTPS**: Should be served over HTTPS when possible for security