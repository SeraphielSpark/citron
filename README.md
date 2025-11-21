Vision UI Library Documentation
Version: 1.0
Author: Michael
Description: A lightweight, modular UI library that provides ready-to-use components and utilities for web projects, including dark mode, modals, toasts, accordions, sliders, chat assistants, notifications, and more.

Table of Contents
Installation
Dark Mode
Toast Notifications
Scroll Reveal
Modals
Character Counter
Countdown Timer
Smooth Scroll
Tabs
Accordion
Image Slider / Carousel
Clipboard Copy
Password Strength Checker
Alert Boxes
Floating Action Button (FAB)
Cookie Consent
Offline Detector
Live Search Filter
Notification Bell
Theme System
Floating AI Chat Assistant

Installation
Include your JavaScript file in your project:
<script src="vision-ui.js"></script>
No dependencies are required. All CSS is automatically injected by the library.

Dark Mode
Toggle dark mode across your website.
Function: visionDarkMode()
Usage:
visionDarkMode();
Features:
Changes background and text colors automatically.
Adjusts button styles for readability.
Works with all components, including modals and alerts.
Shows toast notification: "Dark mode enabled!".


Toast Notifications
Lightweight, floating notifications.
Function: visionToast(message, duration = 3000)
Usage:
visionToast("Data saved successfully!", 4000);
Customizations:
message: Text to display.
duration: Display time in milliseconds (default: 3000ms).


Scroll Reveal
Reveal elements as the user scrolls.
Function: visionScrollReveal()
Usage:
visionScrollReveal();
HTML Example:
<div class="reveal">This will reveal on scroll</div>
Behavior: Adds .reveal-active class when element is in viewport.



Modals
Custom popup modals.
Function: sparkModal(title, bodyText)
Usage:
sparkModal("Welcome!", "This is your first modal");
Features:
Automatic fade-in animation.
Close button (×) to dismiss.
Live Character Counter
Track input length dynamically.
Function: sparkCharCount(inputSelector, counterSelector)
Usage:
sparkCharCount("#message", "#charCount");
HTML Example:
<input id="message" type="text">
<span id="charCount" class="spark-char-counter"></span>

Countdown Timer
Displays countdown to a specific date.
Function: sparkCountdown(targetDate, displaySelector)
Usage:
sparkCountdown("2025-12-31 23:59:59", "#timer");
HTML Example:
<div id="timer" class="spark-countdown"></div>

Smooth Scroll
Animate scrolling to elements.
Function: sparkSmoothScroll(targetSelector, offset = 0, duration = 800)
Usage:
sparkSmoothScroll("#section2", 50, 1000);









Tabs
Switch between tabbed content.
Function: sparkTabs(buttonSelector, contentSelector, activeClass = "active")
Usage:
sparkTabs(".tab-buttons button", ".tab-content");
HTML Example:
<div class="tab-buttons">
  <button>Tab 1</button>
  <button>Tab 2</button>
</div>
<div class="tab-content">Content 1</div>
<div class="tab-content">Content 2</div>


Accordion
Expandable panels.
Function: sparkAccordion(headerSelector, activeClass = "spark-acc-active")
Usage:
sparkAccordion(".spark-accordion");
HTML Example:
<div class="spark-accordion">Header 1</div>
<div class="spark-accordion-panel">Panel 1</div>


Image Slider / Carousel
Automatic sliding images.
Function: sparkSlider(containerSelector, intervalTime = 3000)
Usage:
sparkSlider(".spark-slider", 5000);
Clipboard Copy
Copy text programmatically.
Function: copyToClipboard(text)
Usage:
copyToClipboard("Hello World!");

Password Strength Checker
Dynamic password strength indicator.
Function: sparkPasswordCheck(inputSelector, barSelector)
Usage:
sparkPasswordCheck("#password", "#strengthBar");
HTML Example:
<input type="password" id="password">
<div id="strengthBar" class="spark-strength-bar"></div>

Alert Boxes
Custom popup alerts.
Function: sparkAlert(title, message, duration = 4000)
Usage:
sparkAlert("Warning", "Your session is about to expire", 5000);

Floating Action Button (FAB)
Expandable action buttons.
Function: sparkFAB(mainButtonText, actions = [])
Usage:
sparkFAB("+", [
  { label: "Add", onClick: () => alert("Add clicked") },
  { label: "Edit", onClick: () => alert("Edit clicked") }
]);

Cookie Consent
Show cookie consent popup.
Function: sparkCookies(message, acceptText = "Accept")
Usage:
sparkCookies("We use cookies to improve your experience.");


Offline Detector
Banner for offline detection.
Function: sparkOfflineBanner(message = "You are offline")
Usage:
sparkOfflineBanner();


Live Search Filter
Filter items dynamically.
Function: sparkFilter(inputSelector, itemSelector)
Usage:
sparkFilter("#searchInput", ".item");


Notification Bell
Bell with badge counter.
Function: sparkNotify(count = 0)
Usage:
sparkNotify(5);

Theme System
Dynamic theming using CSS variables.
Function: sparkTheme(theme = {})
Usage:
sparkTheme({
  primary: "#ff5500",
  background: "#111111",
  text: "#fff"
});


Floating AI Chat Assistant
Interactive floating chat widget.
Function: sparkChatAssistant(options = {})
Usage:
sparkChatAssistant({
  title: "Support",
  placeholder: "Ask me anything..."
});


Conclusion
Vision UI Library provides a comprehensive set of modern, customizable components and utilities with built-in dark mode support. All components are modular, easy to use, and lightweight, making it ideal for rapid front-end development.
