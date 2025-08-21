⏰ Analog Clock using HTML, CSS, and JavaScript

This project is a simple Analog Clock built with HTML, CSS, and JavaScript.
It dynamically displays the current system time with animated clock hands for hours, minutes, and seconds.

📌 Features

Real-time clock that updates every second.

Smooth rotation of second and minute hands.

Hour and minute values displayed in text format.

Clock spikes around the dial for better readability.

Pure vanilla JavaScript (no external libraries required).

🛠️ How It Works

The script generates 60 spikes (like tick marks) around the clock for both minutes and seconds.

JavaScript retrieves the current time using the Date() object.

The hour, minute, and seconds values update dynamically every second using setInterval().

CSS variables (--rotate and --dRotate) control the rotation of the clock hands.

📂 Project Structure
📁 analog-clock
 ┣ 📄 index.html   # Main HTML file
 ┣ 📄 style.css    # Styling for the clock
 ┣ 📄 script.js    # JavaScript logic (time updates & animation)
 ┗ 📄 README.md    # Project documentation

🚀 Usage

Clone or download this repository.

Open the index.html file in your browser.

The analog clock will appear and start running immediately.

🖼️ Preview

The clock displays:

Hour hand (current hour in text format).

Minute hand (current minute in text format).

Second hand (rotates around the clock).

Spikes (like real clock marks).

📜 Code Highlights (script.js)
// Update clock every second
setInterval(getTime, 1000);

// Fetch current time
function getTime() {
  let date = new Date();
  let s = date.getSeconds();
  let m = date.getMinutes();

  // Update hour and minute text
  hour.textContent = date.getHours();
  minute.textContent = m;

  // Rotate hands
  minutes.style = `--dRotate:${6 * m}deg`;
  seconds.style = `--dRotate:${6 * s}deg`;
}

✅ Requirements

Any modern browser (Chrome, Firefox, Edge, etc.).

No external dependencies.

✨ Future Improvements

Add hour hand rotation.

Add digital clock display.

Dark/Light mode themes.

Responsive design for mobile view.

📄 License
This project is open-source and free to use for learning and development.

📷 ScreenShot

<img width="1830" height="882" alt="Screenshot 2025-08-21 231852" src="https://github.com/user-attachments/assets/6c2bdb0b-b9de-4c88-9700-7716a8ec2c8a" />
