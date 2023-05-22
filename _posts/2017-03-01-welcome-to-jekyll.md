---
title: "Danker Rust Server"
layout: post
---

The Danker Rust Server was a project I created for multiple verified Twitch streamers. It was a [Rust](https://rust.facepunch.com/) server that I had hosted with many custom plugins as well as a powerful website.

I have published all of the plugins I have created as well as a brief description of what each of them do to [here.](https://github.com/MrAuro/rust-plugins)

Creating this project was enjoyable, and I am proud of the work I have done. I look forward to creating more projects like this in the future.

---

## Website

I used **Remix, React, Typescript, Mantine, Redis, and MongoDB**. For authentication, I used Remix-Auth, alongside OAuth providers for Twitch, Steam, and Discord. A Discord bot would also invite the user to the Discord server and grant them a role when they were approved. Below are some screenshots showing the website's capabilities.

1. Homepage with a randomly picked background graphic
   ![Homepage](https://i.mrauro.dev/ND-homepage.png)
2. Connect page showing users how to connect to the server
   ![Connect page](https://i.mrauro.dev/ND-connect.png)
3. Leaderboard (connects with the Leaderboard and PvpAction custom made Rust plugin)
   ![Leaderboard](https://i.mrauro.dev/ND-leaderboard.png)
4. Stats modal breaking down a user's points
   ![Stats modal](https://i.mrauro.dev/ND-stats.png)
5. Posts page where admins can create posts and users can upvote/downvote them
   ![Posts page](https://i.mrauro.dev/ND-posts.png)
6. Admin page for users to be approved and whitelisted by an admin
   ![Manage users](https://i.mrauro.dev/ND-manageusers.png)
7. Create post page where admins can use rich formatting to enhance their message
   ![Create post](https://i.mrauro.dev/ND-createpost.png)

---

## Plugins

Below is a brief description of what each plugin does (source code is available [here](https://github.com/MrAuro/rust-plugins)). All code was written in **C#** using the **Oxide API**.

### **PvpAction**

An improved version of my PvpAtNight plugin which communicates to the Danker Rust Server web app to track player's kills. This plugin improves the drop rates at night, gives rewards for PVP at night, and gives rewards to players at certain T2+ monuments. It also displays a UI element letting the player know that they are in a PVP area. There is also a Purge that randomly happens which allows for PVP.

### **Leaderboard**

Listens to many events and sends them to the Danker Rust Server web app for processing.

### BuffHorses

Finds horses and improves the stats to make them more usable.

### CheckForHeli

Checks if there is a Minicopter on the helipad for Small and Large Oil Rigs and messages the player if one is found.

### ChinookCrates

Automatically starts unlocking the crates that drop from Chinooks.

### LimitTemp

Sets the minimum and maximum temperatures to be less annoying.

### LockProgression

Makes use of the Oxide permissions system to allow admins to lock and unlock certain features that would cause fast progression.

### MapTeleport

Fetches the location where a player has a map marker on and teleports them there. (I didn't know there was an in-game command for this before creating it :p)

### PvPAtNight

A less feature-rich version of PvpAction.

### SetDay

Allows admins to set the time to day.

### TrollSignal

Allows an admin to give themself a smoke grenade with a supply signal skin on it.

## Welcome

Welcomes users when they join the server.

## Wheel

Does nothing; was meant for testing.
