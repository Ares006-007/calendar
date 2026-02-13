<img width="503" height="454" alt="image" src="https://github.com/user-attachments/assets/249e26f3-872a-4948-841d-2990024344fa" />

# JavaScript Calendar UI

A simple, responsive month-view calendar built with **HTML**, CSS, and vanilla JavaScript.
## Features

- Displays current month, year, and all days laid out in a 7‑column grid.
- Previous and next icons to navigate across months dynamically.
- Highlights the current day and visually distinguishes days from previous/next months. 
- Centered card layout with modern typography using the Poppins Google Font. 
- Dark page background with a white calendar card and hover effects on days. 

## Tech Stack

- HTML5 for structure. 
- CSS3 (flexbox, box‑shadow, custom styling) for layout and design. 
- Vanilla JavaScript Date API for calendar logic and month navigation. 

## Project Structure

- `index.html` – Markup for the calendar wrapper, header (month/year + icons), and weeks/days lists.
- `style.css` – Styles for body centering, wrapper card, icons, weeks, and days with active/inactive states. 
- `script.js` – Logic to render days, handle previous/next month clicks, and highlight today.  

## Getting Started

1. Clone or download this repository.  
2. Open `index.html` directly in your browser, or serve via a local server (for example, VS Code Live Server).
3. Use the left/right icons to move between months. 
## How It Works

- Uses `new Date()` to get the current year and month.   
- Calculates:
  - First weekday of the month  
  - Last date of the current month  
  - Last date of the previous month  
  - Last weekday of the current month 
- Populates the `.days` `<ul>` with `<li>` elements for:
  - Trailing days from the previous month (`inactive`)  
  - All days of the current month (with `active` on today)  
  - Leading days from the next month (`inactive`) 
- Updates the `.current-date` element text with the month name and year using a `months` array.

## Customization

- Switch to a dark calendar card by toggling the commented `background`, `color`, and `border` lines in `.wrapper`. 
- Adjust dimensions by changing the `width` of `.wrapper` or font sizes of `.calendar li`.   
- Modify highlight color by changing `.days li.active::before` background.

## License

This project is open for learning and personal use. Feel free to modify and integrate it into your own projects.
