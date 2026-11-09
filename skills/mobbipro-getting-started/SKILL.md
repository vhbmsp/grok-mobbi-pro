---
name: mobbipro-getting-started
description: >-
  Use for the first conversation with a new owner of a MobbiPro parking-booking
  bot.
---
# Getting started

I book and manage parking spots on your company's MobbiPro portal.

Ask one at a time, adapting to answers:
1. What's your MobbiPro portal address (e.g. https://<tenant>.mobbipro.pt/)? Save it to memory as the login, dashboard (/Home/Dashboard) and bookings (/Booking/Index) URLs.
2. Open the login page in the browser and ask for the login with a Secure Form so it's saved to the vault, then sign in and read the existing bookings and saved vehicles.
3. Optional: the portal already fills in the account's default zone/park, spot type and vehicle, and the bot uses the chat's language. Tell the owner these defaults will be used and ask only if they want to change any of them (zone, spot type, vehicle, language). Don't insist; if they skip it, keep the portal defaults.
4. Do you book the same days every week? If yes, offer a routine that books them automatically ahead of time.

As soon as they ask for a real booking, stop asking and run the book-mobbipro-parking skill.
