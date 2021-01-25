---
title: If not Signal now, when?
tags: [tech]
categories: [Tech]
style: 
layout: post
color: 
date: '2021-01-10 8:12:36 +0530'
description: Why you should switch to Signal, iMessage, Telegram, or other secure messaging app alternatives to WhatsApp.
---

*This is a brain dump of notes from conversations I've been having with people since WhatsApp updated its Terms & Conditions for Feb 8, 2021 on why people should switch to Signal and Telegram (and get rid of Facebook Messenger while you're at it). It will probably be updated.*

Many people have have written better resources about secure messaging apps. The problem is the people asking me, "Why not WhatsApp?" don't read them. 

The other problem is that too many people use WhatsApp and the cost of switching seems too high. 

### Why shouldn't I use Whatsapp?

![Apple 'App Privacy' labels in App Store for WhatsApp and iMessage](https://specials-images.forbesimg.com/imageserve/5ff07f1e39ef1e72ed404595/960x0.png?fit=scale)



WhatsApp is updating its Terms and Conditions as of [February 8, 2021](https://www.whatsapp.com/legal/updates/privacy-policy/?lang=en) to explicitly pass on your data to Facebook. You will not be able to use the app if you do not explicitly agree.

*What's the big deal?*
I will do another post about this when I have the time. But there's lots of literature on why WhatsApp and Facebook having a mountain of your data is no good.

*But wait, isn't WhatsApp end-to-end encrypted and that means the app can't see what I send to other people?* Yes, it WhatsApp uses an opensource end-to-end encryption protocol shared by other apps, including Signal (one of the best choices for secure private messaging apps). This means that the messages you send to other people are sent from your device to your contacts' devices, and that at no point during the sending process is the data passed to other sources (think of someone tapping your phone line). There are two problems to WhatsApp's end-to-end encryption:

1. The code for WhatsApp is not opensource, which means the public cannot look at the code to check for backdoors. You have to trust the company to really be doing end-to-end encryption and other privacy features and not secretly listening in to your conversations.
2. The new Terms & Conditions do not pass your messages. They pass your user data. This is now documented in Apple's App Store showing the types of data apps collect from your device (this [article has a list of data WhatsApp collects](https://www.forbes.com/sites/zakdoffman/2021/01/03/whatsapp-beaten-by-apples-new-imessage-update-for-iphone-users/?sh=e06515836234) and [diagram of what Facebook Messenger collects](https://twitter.com/signalapp/status/1346258308496150528/photo/1)) These include things like contacts and geolocation, device marker, amongst other things. Together, these pieces of information map out the outline of you as an individual, and nonetheless exposes you and your contacts to Facebook. Even if Facebook doesn't know what you are saying, it knows who you are talking to, when, and how frequently. 

![Signal, iMessage, Whatsapp, Facebook Messenger personal data collection chart](https://specials-images.forbesimg.com/imageserve/5ff07f779f9392c3af404599/960x0.png?fit=scale)

### OK, so what are alternative messaging apps?

The list (in order of security and privacy) is:

| App  | Chat | Group chat | Video/call | Group video call |
| ---- | ---- | ---------- | --- | ---------- |
| [Signal](https://signal.org/download/) | Yes | Yes | Yes  |5 Max |
| [Threema](https://threema.ch/en/) | Yes | Yes | Yes  |  Yes |
| [Wire](https://wire.com/en/download/) | Yes | Yes | 25 max |12 Max |
| [Wickr](https://wickr.com/product-tiers/) | Yes | Yes | Yes  | 100 Max |
| [Telegram](https://telegram.org) | Yes | Yes | Yes  | -- |
| iMessage| Yes | Yes | Yes  | Yes |

My recommendation is **Signal**. Most people will have **Telegram** and everyone with an iPhone has **iMessage**, so both are convenient alternatives.

The short list of considerations for getting another app are:
- Is it open-source? If yes, then it means the code is publicly reviewed to ensure that the service really is end-to-end encrypted, collects only the data it says it does (if any), and is actually secure (i.e. no security vulnerabilities).
- How many other people are using it? **Telegram** is top for adoption, which also means it's probably the most convenient for you to switch -- most of your WhatsApp friends will probably be there as well.
- How private do you want to be? For example, if you do not want your account to require a phone number or account to join a video call. 

On a similar note, there are more private video conferencing solutions than using Google Meet or Zoom. The two best solutions are [Whereby](https://whereby.com/) and [Jitsi](https://jitsi.org/). If it's a smaller group, you can use [Signal](https://signal.org/download/) for up to 5 people. [Threema](https://threema.ch/en/), [Wire](https://wire.com/en/download/), and  [Wickr](https://wickr.com/product-tiers/) are secure workplace messaging and video solutions.

If you want to learn more about the factors that should be considered for secure messaging apps, check out this [mega chart of factors](https://www.securemessagingapps.com/) (should be updated soon in 2021).

Pro tip question: Is it secure-by-design? Security is usually defined as whether someone can 1) get into your data, 2) modify your data, 3) has the opportunity to do either of the two. Security isn't just end-to-end encryption, but also how an app is designed. For this reason, I *do not like Telegram*. Telegram is good for privacy, but not security. It offers privacy through annonymity -- by hiding Channel administrators and allowing people to be searched by user account rather thann phone number. However, Telegram is *not secure by default*. The chats you start on Telegram *are not end-to-end encrypted* because they are stored in the cloud. To enable encrypted chats, you must manually start a **Secret chat** with someone. A secret chat will not be seen on your Telegram desktop app because it is only sent to your smartphone, and not passed into the cloud. This design flaw means that majority of people are not actually talking securely over Telegram. 

### Misconceptions about switching from WhatsApp to another messaging service

**I have to get used to a new app.**

Almost all messaging apps work the same way. They have contacts, messages, and groups. Most of the other messaging apps actually have more features than WhatsApp. Telegram grew big because of its stickers (which Signal also has). Telegram and Signal both have self-destruct timers that you can turn on in case you want to talk about a sensitive topic (or sharing a password) and remove the messages after a certain amount of time (1 hour, 1 day, 1 week).

**But no-one is using these other apps.**
You'd be surprised how many people are (for example, if you're an iPhone user, you can reach all your other iPhone friends with iMessage). 

On your device, you can grant your messaging app of choice access to your contacts, you will be able to see who else is using the app and start messaging them. On Signal, you can turn off access to contacts once you're done messaging the people you want to reach. If you turn off an app's access to your contacts, it means they will not automatically include the names of people using the app, but you can still manually add them to a chat by copying and pasting their phone number. For people not using the app, create a group and share the link to the group to invite them.

### Security requires design as much as tech

**Why Telegram is not secure by design**

There is a term called "security by design" or "secure by design". This principle is what differentiates Signal from Telegram. Telegram, to me, fails the "security by design" test because it defaults to non-encrypted chats. If you want end-to-end encryption on Telegram, you must click into a chat with someone, you need to take the following steps:
1. Start a chat with them
2. Click on their name at the top of your chat screen
3. Click "More"
4. Click "Start Secret Chat"
5. Wait for the other person to go online to activate the secret chat room

Telegram will only allow you to start typing once the other person is online. You know you are using a secret chat when you see a *green lock* beside the name of the preson you're talking to.

It takes 5 steps for you to have a secure, end-to-end encrypted chat in Telegram.

End-to-end encrypted chats in Telegram are *not accessible from your desktop*. This is a massive inconvenience to many people, which means many people will just opt not to use end-to-end encryption. That's a security fail. Signal does not have this problem -- both your mobile and your desktop messages are encrypted.

Secure by design means that in addition to having security features such as encryption, an app should be designed in such a way as to make security and privacy a default. Security by design as a principle includes can include:

- an app's default settings (automatically end-to-end encrypted)
- features (such as message timers)
- asking for explicit permission (*not* automatically adding a person's contacts, but instead asking for authorization)
- allowing users to switch off permissions (such as access to your image gallery)
- notifications (such as warnings when a user lets a third-party app access certain files, or if someone takes a screenshot of the chat)

No app has every single feature. But you can choose the features that matter to you, or the bottom line features that you must have for the services you use. In the end, it is a question of the risk threshold you are willing to accept. For example, you may continue to use WhatsApp, but choose to limit who you talk to on it. 

**Why are desktop messaging apps sometimes end-to-end encrypted and sometimes not?**

*Disclaimer: Please keep in mind some of the concepts here may be simplified to help understand a basic concepts.*

Why is Telegram not encrypted for desktop, but Whatsapp and Signal are? A clue lies in how you can use the apps. If your phone is dead, your WhatsApp web will not work either but your Telegram desktop/web will. Whatsapp is designed in such a way where a message someone sends goes only to your phone, and from your phone, the message is pushed into your web browser (think of it like a forwarding service). But if your phone is gone, it is like the first letterbox is gone, so there is no further place to forward to. 

Telegram works on desktop even when your phone is dead because the message are sent up to a cloud server, which your computer can access in parallel to your phone. This is why, when you turn on a secret chat on Telegram, your desktop version cannot access the messages -- Telegram did not design its desktop service to be a forwarding service.

Why does Signal work when your phone is dead? Signal uses encryption to connect each of your devices individually. If you authorize your desktop, then it is treated as another encrypted recieiving end. 

**Signal is only as safe as your keyboard.**

In reality, no service connected online is 100% safe. As long as there is a way for information to be transmitted, there is a way for an attack to occur. 

In the case of Signal -- true of *all messaging apps, and every app using a keyboard* -- a weak link is the **keyboard**. If you are using a third-party keyboard, chances are you had to accept the Terms & Conditions in order to use it, which may contain rights to monitor your typing. This means that the keyboard provider can log everything you type, and in theory extract all your messages. This issue has been raised by the China's top tech & DIY YouTuber, opensource advocate and activist [Naomi Wu 机械妖姬](https://twitter.com/RealSexyCyborg/status/1197695344575799296). Naomi Wu also [goes at length to explain why IME (aka keyboards) apps make Signal unsafe for users in China](https://community.signalusers.org/t/signal-should-warn-users-who-are-likely-using-insecure-ime-apps/10272). The issue is worse usually for [Android phones, where users tend to do more customizations](https://github.com/signalapp/Signal-Android/issues/6985), but could be equally true of iPhones as well -- and as a side note, you can rethink whether you want to use the Google Keyboard too.




*This document may be updated occasionally.*
