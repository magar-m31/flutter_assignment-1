# Flutter Chat Application UI

A beautiful and responsive chat application UI built with Flutter, replicating a modern messaging interface with all essential chat features.

## Features

### 🎨 UI Components

1. **App Bar**
   - Back arrow navigation
   - Circular user avatar with initials
   - User name and online status
   - Call and video call buttons

2. **Date Separator**
   - Stylized "Today" label with chip design
   - Centered positioning with light background

3. **Chat Messages**
   - **Outgoing Messages**: Green bubbles aligned to the right
   - **Incoming Messages**: White/light grey bubbles aligned to the left
   - Rounded corners with flattened bottom corners for realistic chat appearance
   - Timestamps displayed below each message
   - **Audio Message**: Special bubble with play button, waveform visualization, and duration

4. **Message Input Area**
   - Attachment icon (paperclip)
   - Expandable text input field with placeholder text
   - Picture, camera, and microphone icons
   - Clean design with rounded corners

## Technical Implementation

### Widget Hierarchy

```
ChatApp (MaterialApp)
├── ChatScreen (StatefulWidget)
    └── Scaffold
        ├── AppBar
        │   ├── Leading (Back Button)
        │   ├── Title (Avatar + User Info)
        │   └── Actions (Call & Video Icons)
        └── Body (Column)
            ├── Expanded (ListView.builder)
            │   ├── Date Separator
            │   └── Message Bubbles
            │       ├── Regular Messages
            │       └── Audio Messages
            └── Message Input Area
                └── Row (Input + Icons)
```

### Key Classes

- `ChatApp`: Main application widget with Material theme
- `ChatScreen`: Stateful widget managing the chat interface
- `ChatMessage`: Model class for message data
- `_ChatScreenState`: State management for the chat screen

### Styling Features

- **Material Design 3**: Modern Flutter theming
- **Responsive Layout**: Adapts to different screen sizes
- **Color Scheme**: Green for outgoing, white for incoming messages
- **Typography**: Clean, readable text with proper sizing
- **Shadows**: Subtle elevation for message bubbles
- **Animations**: Smooth scrolling and interactions

## Getting Started

### Prerequisites

- Flutter SDK (3.0 or higher)
- Dart SDK
- Android Studio / VS Code
- iOS Simulator / Android Emulator

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/flutter_assignment_1.git
   cd flutter_assignment_1
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   flutter run
   ```

### Testing

Run the test suite:
```bash
flutter test
```

Run code analysis:
```bash
flutter analyze
```

## Project Structure

```
lib/
├── main.dart                 # Main application entry point
test/
├── widget_test.dart          # Widget tests
```

## Sample Data

The application includes sample chat messages to demonstrate:
- Regular text messages (both incoming and outgoing)
- Timestamps
- Audio message with waveform visualization
- Proper message alignment and styling

## Development Notes

1. **Quick Setup**: Built with core Flutter widgets - no external packages needed
2. **Iterative Development**: Code structure evolved as features were added
3. **Real-world Considerations**: Added TODOs and placeholder functionality for future implementation
4. **Performance**: Uses ListView.builder for smooth scrolling with many messages
5. **Developer Experience**: Includes debug helpers and placeholder implementations

## Future Enhancements

- [ ] Message sending functionality
- [ ] Real-time messaging with WebSocket
- [ ] Image and file sharing
- [ ] Audio recording and playback
- [ ] Message reactions and replies
- [ ] User authentication
- [ ] Database integration

## Assignment Requirements Fulfilled

✅ **App Bar**: Back arrow, user avatar, name, status, call/video icons  
✅ **Date Separator**: "Today" label with styling  
✅ **Chat Messages**: Incoming and outgoing with proper alignment  
✅ **Message Bubbles**: Rounded corners, timestamps, proper colors  
✅ **Audio Message**: Play icon, waveform, duration display  
✅ **Input Area**: Attachment, text field, camera, picture, mic icons  
✅ **Widget Tree Diagram**: Complete hierarchy visualization  
✅ **Clean Code**: Well-structured, documented, and maintainable  

## Screenshots

The application creates a pixel-perfect replica of modern chat interfaces with:
- Professional color scheme
- Intuitive user interactions
- Clean and minimal design
- Responsive layout

## License

This project is created for educational purposes as part of a Flutter UI assignment.

## Author

Created as part of Flutter UI Assignment - Chat Application

---

**Note**: This is a UI-only implementation focusing on design and layout. For a complete chat application, additional backend integration and real-time messaging functionality would be required.
