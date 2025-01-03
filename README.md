# Flutter Expense Tracker

## Overview
Flutter Expense Tracker is a mobile application built using Flutter to help users efficiently manage their daily expenses. With this application, users can add, view, categorize, and analyze their expenses through an intuitive and user-friendly interface.

## Features

- **Expense Listing**: View all expenses with details such as title, amount, date, and category.
- **Add New Expenses**: Add new expenses using a modal form with fields for title, amount, date, and category.
- **Expense Categories**: Categorize expenses as Food, Travel, Leisure, or Work.
- **Data Visualization**: Visualize expense distribution through a chart.
- **Dark and Light Themes**: Support for both light and dark themes.
- **Undo Deletion**: Option to undo expense deletions via snack bars.

## Project Structure

```plaintext
lib/
├── main.dart                 # Entry point of the application
├── models/
│   └── expense.dart          # Data model for expenses
├── widgets/
│   ├── expenses.dart         # Main widget managing the expense tracker
│   ├── new_expense.dart      # Modal to add new expenses
│   ├── chart/
│   │   ├── chart.dart        # Widget for expense visualization
│   │   └── char_bar.dart     # Widget for individual chart bars
│   └── expenses_list/
│       ├── expenses_list.dart # Widget for listing expenses
│       └── expenses_item.dart # Widget for individual expense items
```

## Widgets

### 1. **Main Widget**
`main.dart`
- Initializes the application.
- Configures themes (light and dark).
- Sets `Expenses` as the home screen.

### 2. **Expense Management**
`expenses.dart`
- Manages the list of expenses.
- Handles adding, removing, and undoing expense deletions.

`expense.dart`
- Contains the `Expense` and `ExpenseBucket` classes.
- Defines the structure and operations of an expense.

### 3. **Adding Expenses**
`new_expense.dart`
- Modal form to input details for a new expense.
- Fields include title, amount, date, and category.

### 4. **Listing Expenses**
`expenses_list.dart`
- Displays a scrollable list of expenses.
- Integrates the `ExpenseItem` widget.

`expenses_item.dart`
- Represents a single expense in the list.
- Displays title, amount, date, and category icon.

### 5. **Visualization**
`chart.dart`
- Aggregates and visualizes expenses by category.
- Dynamically adjusts based on expense data.

`char_bar.dart`
- Individual bar component for the chart.

## Themes

- **Light Theme**: Bright and minimalistic UI.
- **Dark Theme**: Enhanced contrast for low-light environments.

Custom color schemes are defined in `main.dart` using Flutter's `ColorScheme`.

## How to Run

1. **Prerequisites**:
   - Install Flutter SDK.
   - Set up an IDE (VSCode, Android Studio, etc.).
   - Configure a device or emulator for testing.

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/AlonaLaskar/expense-tracker.git
   cd expense-tracker
   ```

3. **Install Dependencies**:
   ```bash
   flutter pub get
   ```

4. **Run the App**:
   ```bash
   flutter run
   ```

## Future Enhancements

- Add persistent storage using local databases (e.g., SQLite).
- Implement filtering and sorting for expenses.
- Introduce monthly and yearly reports.

