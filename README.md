# Travel Tracker

A web application that allows users to track the countries they have visited by marking them on an interactive map.

---

## 📍 About the Project

**Travel Tracker** is a web application that allows users to keep a visual record of the countries they have visited. Users can add countries by name, and the application dynamically highlights those locations on an interactive SVG world map. It also keeps track of and displays the total number of countries visited.

This project was created to combine backend logic with a visually engaging frontend, demonstrating full-stack development skills using **Node.js**, **Express**, **PostgreSQL**, **EJS**, and **custom JavaScript/CSS**. The interactive map provides a rewarding and intuitive way for users to visualize their travel history.

Whether you're a travel enthusiast or building your own bucket list, **Travel Tracker** makes it simple and fun to document your global adventures.

---

Let me know if you’d like to add screenshots, GIFs, or a live demo badge to enhance your README!


## Features

- Add countries to your visited list by entering the country name
- Interactive SVG world map that highlights visited countries
- Displays the total count of visited countries
- Responsive design that works on mobile and desktop devices

## Technologies Used

- **Backend**: Node.js with Express.js
- **Database**: PostgreSQL
- **Frontend**: HTML, CSS, JavaScript
- **Templating**: EJS
- **Styling**: Custom CSS

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/travel-tracker.git
   cd travel-tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up your PostgreSQL database:
   - Create a database named `world`
   - Create a table named `visited_country` with a `country_code` column
   - Create a table named `countries` with `country_code` and `country_name` columns

4. Configure your database connection in `index.js`:
   ```javascript
   const db = new pg.Client({
     user: "postgres",
     host: "localhost",
     database: "world",
     password: "your-password",
     port: 5432,
   });
   ```

5. Start the application:
   ```bash
   node index.js
   ```

6. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

## Usage

1. Enter a country name in the input field
2. Click "Add" to add the country to your visited list
3. The map will automatically update to highlight the country
4. The total count of visited countries will be displayed at the bottom

## Project Structure

```
travel-tracker/
├── public/
│   └── styles/
│       └── main.css       # CSS styles
├── views/
│   └── index.ejs          # Main view template
├── index.js               # Server and application logic
├── package.json           # Project dependencies
└── README.md              # This file
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

