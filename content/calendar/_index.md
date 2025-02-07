---
title: "Calendar"
description: ""
summary: ""
date: 2024-11-06T12:55:56-08:00
lastmod: 2024-11-06T12:55:56-08:00
draft: false
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
<style>
      .col-xl-8 {
          width: 95%;
      }

      .calendar-container {
          display: flex;
          justify-content: center;
          align-items: flex-start;
          width: 100%;
          max-width: 1200px;
          margin: 0 auto;
          padding: 20px;
      }

      iframe {
          border: 3px solid #ccc; /* Grey border */
          border-radius: 12px; /* Rounded edges */
          box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
          width: 100%;
          height: 70vh; /* Scales dynamically with viewport */
          min-height: 400px; /* Prevents it from getting too small */
          max-height: 800px; /* Prevents excessive stretching */
      }

      /* Tablet Adjustments */
      @media (max-width: 1024px) {
          .calendar-container {
              padding: 10px;
          }

          iframe {
              height: 65vh;
              min-height: 400px;
              max-height: 700px;
          }
      }

      /* Mobile Adjustments */
      @media (max-width: 768px) {
          .calendar-container {
              padding: 5px;
          }

          iframe {
              height: 60vh;
              min-height: 350px;
              max-height: 600px;
          }
      }

      /* Smallest Screens */
      @media (max-width: 480px) {
          .calendar-container {
              flex-direction: column;
              padding: 5px;
          }

          iframe {
              height: 55vh;
              min-height: 300px;
              max-height: 500px;
          }
      }
</style>

<div class="calendar-container">
  <iframe src="https://outlook.office365.com/owa/calendar/e35f338d59e243b586b9cae6af358f0c@bellevuecollege.edu/166d130b7fff43c6983e453635e1b8455312721504574280041/calendar.html" scrolling="yes"></iframe>
</div>
