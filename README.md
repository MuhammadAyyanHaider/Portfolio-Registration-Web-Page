Portfolio-Registration-Web-Page
A responsive HTML5, CSS3, and JavaScript university lab assignment featuring a creative portfolio landing page and an interactive registration form with custom client-side validation.

University Portfolio & Registration Web Page
A responsive, multi-page frontend web application developed as part of a university lab assignment. This project consists of a personal portfolio showcase and an interactive registration form, built using clean HTML5, CSS3, and native JavaScript.

Developer Information
Name: Muhammad Ayyan Haider

Roll Number: 045 (Section 6A)

Program: BS Computer Science (6th Semester)

Institution: University of Central Punjab (UCP)

Project Overview
This project serves as a structured demonstration of core frontend web technologies. It is divided into two primary pages connected via a clean navigation bar:

1. Personal Portfolio (index.html)A landing page designed to showcase a creative professional profile.  Hero Section: Features a profile image alongside a bio detailing design focus and user-centric problem-solving.  Interactive Gallery: Responsive grid layout showcasing artistic work with hover effects and scaling animations.  Modern Aesthetic: Styled with a dark, sleek color palette using deep violets and golds.
2.  Interactive Registration Form (registrationForm.html)A functional user registration layout with native and custom form validations.  Input Fields: Collects structured data using specialized HTML5 fields including Name (pattern-restricted to letters/numbers), Email, Password, Telephone, Date of Birth, City, Favorite Color, and Profile Picture uploads.  Custom Form Validations:Strict numeric restriction on the Phone field via JavaScript.  Event-driven Email validation to ensure the presence of the @ symbol before submission.

Technologies UsedHTML5: Semantic structuring (e.g., <header>, <section>, <nav>, <footer>).  CSS3: Flexbox and Grid layouts, linear gradients, transitions, and hover animations.  JavaScript: DOM manipulation, custom event listeners (keypress, submit), and validation logic.  

File Structure
├── index.html            # Portfolio landing page
├── registrationForm.html # Registration form with JS validations
├── profile.png           # Profile avatar used in Hero section
├── art1.jpg              # Gallery image 1
├── art2.jpg              # Gallery image 2
├── art3.jpg              # Gallery image 3
├── art4.jpg              # Gallery image 4
└── art5.jpg              # Gallery image 5

Features & Validation LogicResponsive Grid: The artwork gallery automatically adjusts columns using CSS Grid (repeat(auto-fit, minmax(200px, 1fr))).  Instant Numeric Filtering: The phone input instantly rejects any non-numeric character during typing:  

Javascript:
phoneInput.addEventListener('keypress', function(e) {
  if (!/[0-9]/.test(e.key)) {
    e.preventDefault();
  }
});

Email Safety Check: Prevents submission and alerts the user if the standard @ separator is missing in the email field.  
