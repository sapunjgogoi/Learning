# Learning
Training Of Git &amp; Github

Author : Sapun Jyoti Gogoi

This generator is a lightweight tool designed to produce non-sequential, collision-resistant identifiers. It is particularly useful for temporary session IDs, database keys for small projects, or unique filenames.

The logic relies on two distinct layers of data to ensure the number is truly unique:

Temporal Precision (The Prefix): It uses Date.now(), which captures the number of milliseconds elapsed since the Unix Epoch (January 1, 1970). Because time only moves forward, the first 13 digits of your ID will never repeat.

Random Entropy (The Suffix): To prevent a "collision" (two IDs being created at the exact same millisecond), the script appends a 5-digit random integer. This creates a safety buffer that allows for hundreds of IDs to be generated per second without overlap.

Core Features
Zero Dependencies: It uses pure HTML5, CSS3, and Vanilla JavaScript—no external libraries or frameworks are required.

Instant Feedback: Includes a small UI "flash" effect using setTimeout to let the user know a new number has been successfully generated.

Responsive Design: The CSS uses Flexbox and relative units, ensuring the generator looks good on both desktop monitors and mobile screens.
