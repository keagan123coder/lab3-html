# Tunyas Airlines Website
# Tunya Airlines 

![Tunya Airlines Logo](images/airline-logo.png)

## Group Members
- Keagan Mataga (2021457567)
- Erick Halale (2021475573)
## Project Description
 Tunya Airlines website is a simple three-page responsive site built with HTML and CSS. The project features a home page introducing the airline, a services page with an interactive flight booking form, and a contact page with a message submission form. designed all pages to work perfectly on both mobile devices and computers.

The website uses basic HTML form elements like dropdown menus, radio buttons, and checkboxes in the booking form for flight selection. For layout, i implemented CSS Flexbox and Grid to create responsive designs that adapt to different screen sizes. Simple CSS animations enhance button interactions, while media queries ensure proper display across devices. The entire project was built without JavaScript to maintain simplicity.

Developed by Keagan Mataga (2021457567), this project includes all necessary files: index.html (home), services.html (booking), contact.html (contact form), style.css (styling), and an images folder for graphics. 


## summery of features used
<!-- 
  HTML SELECTORS USED:
  - <select> for flight class dropdown
  - <input type="radio"> for trip type
  - <input type="checkbox"> for add-ons
  - <input type="date"> for calendar picker
  - <input type="number"> for passengers
  - <input type="text/email"> for contact form
-->
/* 
  CSS FEATURES IMPLEMENTED:
*/

/* FLEXBOX LAYOUTS */
.navbar, .form-group, .features {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: space-between;
}

/* CSS GRID SYSTEMS */
.services-grid, .flight-options {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}

/* MEDIA QUERIES */
@media (max-width: 768px) {
  /* Mobile adjustments */
  header { flex-direction: column; }
  .features { grid-template-columns: 1fr; }
}

/* ANIMATIONS & EFFECTS */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

.cta-button {
  transition: all 0.3s ease;
  animation: fadeIn 0.8s both;
}

.cta-button:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

/* FORM VALIDATION STYLES */
input:required {
  border-left: 3px solid #0066cc;
}

input:invalid {
  border-color: #ff4444;
}
