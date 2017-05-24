## Quickride

### Introduction

Quickride is a Telegram bot that brings the Uber expereince to Telegram via the Uber API.

### Goals

The main goal of this bot is to allow Telegram users to easily hail Uber cabs from the app directly.

Telegram is one of the largest messenger apps in the world, and it provides a robust bot API that allows one to easily make a feature-rich bot.

### Use cases and advantages

The bot is useful in situations such as:

- When a user has minimum mobile data available. (Telegram consumes the least amount of data. [[source](https://www.sostariffe.it/news/alternative-a-whatsapp-quanto-consumano-261505/)])
- When the user has limited storage space on the phone.

Telegram is also available on almost every popular platform, this allows one to hail Uber taxis from those platforms.

This bot also makes it faster and easier to hail a taxi due to its simple UX/UI, hence a less steeper learning curve.

### Structure

The bot can support several uses, with each users information stored and notifications sent separately.

**Flow**

1. User sets current position by either sending GPS coordinates from the phones location feature or by using inline mode and manully inputting a known location such as street name.

2. user selects the type of taxi. At the moment only "UberX" and the chapest alternative option is supported. However this may change.

3. User sets destination by either sending GPS coordinates from the phones location feature or by using inline mode and manully inputting a known location such as street name.

4. User receives notifications such as driver/car information, driving arriving status, receipt e.t.c.

### Demonstration

- [Part 1](https://www.youtube.com/watch?v=bqDQnf-7La0) (Authorization)
- [Part 2](https://www.youtube.com/watch?v=9L4WdzsG2QU) (Ordering a taxi)

The demonstartion was done in a sandbox environment. 

**The error handling feature is present. but not demonstrated in the above videos.**

### Privacy policy

[Privacy Policy](https://github.com/kamikazechaser/quickride/blob/master/PRIVACY_POLICY.md)

A link to the privacy policy will be displayed when the user starts the bot.

### F.A.Q

**What Uber taxi types do the bot support?**

The bot primarily support UberX or the cheapest alternative in the user location. If no UberX is available, the cheapest alternative is choosen.

**Does the bot handle errors?**

Absolutely! If a user is already on a trip, and tries to request for another one, it notifies him/her, same apllies to situations such as when a user hasn't confirmed his/her phone number e.t.c. It supports **every** error shown in the making a ride request section of the API documentation.

**What can I do with the bot? (Relative to the native mobile apps)**

- It can display the basic Uber profile information such as name and e-mail address.
- It can order an Uber taxi.

**What can't I do with the bot? (Relative to the native mobile apps)**

- It cannot apply promo codes.
- It cannot set payment methods.*
- It cannot update profile details.
- It cannot display previous trips and their receipts.*
- It cannot rate drivers.
- It cannot open support tickets to Uber.

_* - May be available in the future._

**What OAuth scopes are required?**

- profile
- request 
- request_receipt

### Questions?

If you have any further question, you can reach out to me via telegram @kamikazechaser or Email me at:

- sohailsameja@gmail.com
- sohail@forfuture.tech
