---
name: book-mobbipro-parking
description: >-
  Use when the user asks to book, check or cancel a parking spot on their
  MobbiPro (mobbipro.pt) portal.
---
# Book or cancel parking on MobbiPro

1. Work out the exact date(s) from the user's words ("next Wednesday" = the coming Wednesday) and the interval: All Day, Morning, Afternoon or Custom start/end times. Use the user's usual zone, spot type and vehicle from memory unless they say otherwise.
2. Dispatch a browser task to the portal's bookings page (https://<tenant>.mobbipro.pt/Booking/Index). If it lands on the login page, fill the saved vault login (Username / E-mail, Password), tick Remember me, and log in.
3. Open Book Parking, pick zone, interval, start/end, spot type (CAR/MOTO/BIKE), quantity 1, then the saved vehicle. If the vehicle the user named isn't saved, stop and report the saved list; don't create one.
4. Click Reserve Spot. The portal books straight away and shows a success dialog ("Your reservation was successfully submitted!...") with zone, dates and vehicle plate. Report that text and a screenshot.
5. For checking bookings, read the list on the bookings page (date, time, zone, spot type, status Used/Not Used) without changing anything.
6. To cancel: only when the user asked for that specific booking. On the bookings page find exactly the matching row (date, time window, zone, vehicle); if none or more than one matches, stop and report. Use "Free Permanently" on that row and confirm the prompt "Do you wish to free your spot?" after checking it shows the same time interval. No success message appears; verify the booking is gone from the active list and report with a screenshot.
7. Tell the user the booked or cancelled date, time window, zone and vehicle in one sentence.
