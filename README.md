# To-Do List Application 📝

A modern, fully functional to-do list application with persistent local storage functionality. Built with vanilla HTML, CSS, and JavaScript.

## ✨ Features

- **Add Tasks**: Easily add new tasks with a clean input interface
- **Complete Tasks**: Mark tasks as complete/incomplete with a checkbox
- **Delete Tasks**: Remove individual tasks from your list
- **Filter Tasks**: View All, Active, or Completed tasks
- **Local Storage**: All tasks are automatically saved to your browser's local storage
- **Task Counter**: See how many tasks are remaining at a glance
- **Clear Completed**: Bulk delete all completed tasks at once
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Beautiful UI**: Modern gradient design with smooth animations and transitions
- **Security**: XSS protection through HTML escaping

## 🚀 Quick Start

1. **Clone or download** the project files
2. **Open `index.html`** in your web browser
3. **Start adding tasks!** Your tasks will be saved automatically

## 📁 File Structure

```
/
├── index.html          # HTML structure
├── styles.css          # CSS styling and animations
├── script.js           # JavaScript functionality
└── README.md           # Documentation
```

## 💻 Usage

### Adding a Task
- Type your task in the input field
- Click "Add Task" or press Enter
- Your task appears in the list

### Managing Tasks
- **Check/Uncheck** the checkbox to mark tasks as complete
- **Click Delete** to remove a task
- **Use Filters** (All, Active, Completed) to view different task categories

### Local Storage
- All tasks are automatically saved to your browser's local storage
- Tasks persist even after closing and reopening the browser
- Each task is stored with:
  - Unique ID (timestamp-based)
  - Task text
  - Completion status
  - Creation timestamp

### Clear Completed
- Click "Clear Completed" to remove all finished tasks
- Confirmation dialog prevents accidental deletion

## 🎨 Design Features

- **Gradient Theme**: Purple to violet gradient background
- **Smooth Animations**: Fade-in effects for new tasks
- **Hover Effects**: Interactive buttons and task items
- **Custom Scrollbar**: Styled scrollbar for the task list
- **Mobile Optimized**: Responsive layout for all screen sizes

## 🔧 Technical Details

### Class: TodoApp
The application uses an object-oriented approach with the `TodoApp` class:

**Methods:**
- `init()` - Initialize the application
- `addTodo()` - Add a new task
- `deleteTodo(id)` - Remove a task
- `toggleTodo(id)` - Mark task as complete/incomplete
- `setFilter(filter)` - Change active filter
- `getFilteredTodos()` - Get tasks based on current filter
- `clearCompleted()` - Remove all completed tasks
- `saveToStorage()` - Save tasks to localStorage
- `loadFromStorage()` - Retrieve tasks from localStorage
- `render()` - Update the DOM
- `updateStats()` - Update task counter

### Storage Format
Tasks are stored in localStorage as JSON:
```javascript
[
  {
    "id": 1234567890,
    "text": "Sample task",
    "completed": false,
    "createdAt": "2026-04-20T10:30:00.000Z"
  }
]
```

## 🌐 Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Any modern browser with ES6 support and localStorage API

## 🔒 Security

- **XSS Protection**: User input is escaped before rendering to prevent script injection
- **Input Validation**: Empty tasks are rejected
- **Confirmation Dialogs**: Critical actions require user confirmation

## 📱 Responsive Breakpoints

- **Desktop**: Full layout with optimal spacing
- **Tablet**: Adjusted padding and filter button layout
- **Mobile**: Stacked input elements, full-width buttons

## 🚀 Future Enhancements

Potential features to add:
- Task categories/tags
- Due dates and reminders
- Priority levels
- Local backup/export
- Dark mode toggle
- Task search functionality
- Recurring tasks
- Cloud synchronization
- Task sharing
- Keyboard shortcuts

## 📝 Notes

- Tasks are stored locally in your browser - clearing browser data will delete tasks
- Works offline - no internet connection required
- No personal data is sent to any server
- Each browser/device maintains its own separate task list

## 🎓 Learning Points

This project demonstrates:
- DOM manipulation with vanilla JavaScript
- Event handling and delegation
- localStorage API usage
- CSS animations and transitions
- Responsive design principles
- Object-oriented JavaScript
- ES6 class syntax
- Array methods (filter, find, etc.)
- XSS prevention techniques

---

**Enjoy organizing your tasks!** 🎉