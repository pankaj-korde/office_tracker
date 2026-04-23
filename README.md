# Office Timer ⏰

A modern, mobile-responsive work day timer application to track your 4-hour office shifts with real-time status updates, notifications, and sound alerts.

## Features

✨ **Core Features:**
- ⏱️ **Customizable Timer** - Set any duration (default: 4 hours)
- 🎯 **Preset Options** - Quick presets: 2 min, 5 min, 10 min, 1 hour, 2 hours, 4 hours
- 📊 **Live Status Tracking** - Monitor Swipe-in, Leave by, Elapsed, and Remaining time
- 📈 **Visual Progress Bar** - Real-time progress visualization
- 🔔 **Sound Notifications** - Warning beeps at 1 minute and 10 seconds
- 🔊 **Continuous Sound** - Optional looping alert when time completes
- 📱 **Mobile Responsive** - Works seamlessly on phones, tablets, and desktops
- 🕐 **Live Clock** - Displays current date and time
- 🎊 **Completion Notification** - Beautiful modal alert with custom message
- 🌙 **Dark/Light Theme** - Modern gradient UI with smooth animations

## Getting Started

### Quick Start
1. Open `index.html` in any modern web browser
2. Click "Start" to begin the timer
3. Timer will automatically set to 4 hours
4. When done, you'll see a completion notification

### Changing the Duration
**Option 1 - Preset Buttons:**
- Click any preset button (2 min, 5 min, 10 min, 1 hour, 2 hours, 4 hours)

**Option 2 - Custom Time:**
1. Enter Hours, Minutes, and Seconds in the input fields
2. Click "Set" button or press Enter
3. Click "Start" when ready

## Usage Guide

### Status Panel
- **Swipe-in** - Shows the time you clicked Start
- **Leave by** - Automatically calculated (Swipe-in + Duration)
- **Elapsed** - How much time you've worked
- **Remaining** - Time left to work

### Live Status Indicator
- 🟢 **In Progress** - Green indicator when timer is running
- ✓ **Done** - Red indicator when time is complete

### Controls
- **Start** - Begins the countdown timer
- **Pause** - Pauses the timer (can resume with Start)
- **Reset** - Resets to original duration and clears all data

### Sound Settings
- **Sound Notifications** - Enable/disable warning beeps
  - Beeps at: 1 minute remaining, 10 seconds remaining, completion
- **Continuous Sound** - Enable/disable looping alert when done
  - If enabled, alerts every 2 seconds until you click "Stop Sound"

## Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- Audio support (for sound notifications)

## Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| Edge | ✅ Full Support |
| Mobile Chrome | ✅ Full Support |
| Mobile Safari | ✅ Full Support |

## File Structure

```
index.html          - Complete single-file application
                      (HTML + CSS + JavaScript combined)
README.md           - This documentation file
```

## Features Explained

### ⏰ Timer Functionality
- Default: 4 hours (14,400 seconds)
- Counts down every second
- Accurate timing with JavaScript setInterval
- Pause and resume capability

### 🎨 User Interface
- Beautiful gradient background (#667eea to #764ba2)
- Responsive grid layout for status cards
- Smooth animations and transitions
- Mobile-optimized touch targets
- Large, readable timer display (3.5em on desktop, 2.2em on mobile)

### 📢 Notifications
- **Browser Notification** - Desktop notification when complete
- **Modal Alert** - On-screen completion message
- **Sound Alerts** - Web Audio API for beeps

### 📱 Responsive Design
- Desktop: 500px max-width centered container
- Tablet (600px): Optimized layout and padding
- Mobile (400px): Smaller fonts, flexible buttons

### ⚡ Performance
- Single-file deployment (no external dependencies)
- Lightweight and fast-loading
- Efficient memory usage with interval cleanup
- Local time tracking (no server required)

## Tips & Tricks

### Power User Tips
1. **Keyboard Shortcuts** - Press Enter in time input fields to quickly set custom time
2. **Quick Presets** - Click preset buttons to instantly change duration
3. **Pause & Resume** - Use Pause to take breaks without losing your elapsed time
4. **Mobile Friendly** - Optimized for small screens, easy one-handed operation
5. **Sound Control** - Enable continuous sound to ensure you don't miss the alert

### Workflow Example
1. Arrive at office → Open timer → Click "Start"
2. Swipe-in time automatically captured
3. Work through the day
4. Get warning at 1 minute remaining
5. Get final alert at 10 seconds
6. Completion notification appears
7. Swipe-out and head home!

## Sound Alerts Explained

### Warning Beep (1 minute & 10 seconds)
- Single frequency tone (600 Hz)
- Light notification to prepare for completion

### Completion Sound
- Three ascending beeps (800 Hz → 1000 Hz → 1200 Hz)
- Recognizable and attention-grabbing
- Plays once by default
- Repeats every 2 seconds if continuous sound enabled

## Notification Message

When the timer completes, you'll see:
```
Time Complete!
You can head home now. Great work today!
```

This can be customized by editing the notification HTML in the code.

## Troubleshooting

### Sound not working?
- Check browser volume settings
- Ensure "Sound Notifications" checkbox is checked
- Grant audio permission if prompted
- Try a different browser

### Timer not counting down?
- Make sure you clicked "Start"
- Check browser console for errors (F12)
- Refresh the page if it appears frozen

### Mobile layout issues?
- Try rotating your device
- Use full-screen mode for better experience
- Ensure browser zoom is at 100%

## Security & Privacy

- ✅ No data is sent to any server
- ✅ No cookies or tracking
- ✅ All processing happens locally
- ✅ Completely offline-capable
- ✅ No personal information collected

## Browser Permissions

The app may request:
- **Notification Permission** - For desktop alerts (optional)
- **Audio Permission** - For sound notifications (optional)

You can grant or deny these. The app works without them.

## Limitations

- Requires JavaScript enabled
- Timer will pause if browser tab is backgrounded (focus loss)
- Sound may not work if browser tab is muted
- Desktop notifications require browser permission

## Tips for Best Experience

1. **Keep the page active** - Don't minimize or switch tabs
2. **Enable sounds** - Set up audio for helpful alerts
3. **Use on desktop** - Full HD display recommended
4. **Check browser settings** - Ensure notifications are allowed
5. **Test it first** - Try a short 1-minute timer to verify functionality

## Customization

To modify the timer:

### Change Default Duration
Edit line in script section:
```javascript
let totalSeconds = 4 * 60 * 60;  // Change to desired seconds
```

### Change Notification Message
Edit the notification-box HTML:
```html
<div class="notification-title">Time Complete!</div>
<div class="notification-message">Your custom message here</div>
```

### Change Colors
Edit CSS color variables:
- Primary: `#667eea`
- Secondary: `#764ba2`
- Success: `#4CAF50`
- Warning: `#ff9800`
- Error: `#f44336`

## Updates & Version

**Current Version:** 1.0
**Last Updated:** April 23, 2026

## License

This application is free to use and modify for personal and commercial purposes.

## Support

For issues or feature requests, you can:
1. Check the Troubleshooting section above
2. Review browser console for error messages
3. Try a different browser to isolate issues

---

**Enjoy tracking your work day! 🎯**

Made with ❤️ for productivity
