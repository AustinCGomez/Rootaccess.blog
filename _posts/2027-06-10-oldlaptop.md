---
layout: post
title: "Breathing New Life into my Old Lenovo Laptop: The Journey to Building a Personal Home Lab"
date: 2026-06-10 00:00:00 -0600
tags: [misc]
excerpt: "Breathing life into old electronics"
---

**Breathing New Life into my Old Lenovo Laptop: The Journey to Building a Personal Home Lab**

It was around August in 2014, and I had just graduated from high school and started attending a local community college to begin my post-secondary education journey. I took up a job, which happened to be my first job, at McDonald’s, making minimum wage in my state of Alabama and mostly working the night shifts on the weekends. I didn’t earn much, but I was able to make anywhere from $150 to $280 per month from working there. At this time, I had an old Asus laptop that was on its last legs. It was unfortunately made of plastic and could not go above 4GB of RAM due to limitations put in place by ASUS for this specific laptop. Needless to say, it would have been tough to even repair this laptop or use it for what I wanted to use it for. I really wanted my own laptop and also something I could buy with my own money. That was when I noticed the Lenovo Y50–70 and began to feel like the kid who wanted the Red Ryder BB gun from the movie _A Christmas Story_.

Over the years, the Lenovo Y50–70 aged, and I could definitely start to feel the machine age like fine wine. I used it for everything from homework assignments to gaming, but as games got more advanced, the machine just struggled to keep up. In addition, I was a computer science major at the time, so it was rather difficult to get it to work on more complex projects. Eventually, the laptop was turned off as I moved on to a new desktop PC, and it sat in its protective case for a few years.

It was only in 2025 when I decided to find a purpose for the Lenovo Y50–70. I did not want to throw it away or simply have it stay on my shelf indefinitely, and I felt that I could somehow make use of it. When I opened up the laptop after several years of being dormant, it was very slow but, most importantly, very insecure, as it ran a Windows 7 operating system, which is no longer updated.

**Step 1: Planning a new operating system:**

The first thing that I needed to do was get rid of the Windows 7 operating system before I even thought about connecting it to the internet. It is easy enough to find out what vulnerabilities exist for this current operating system. I did consider using it as a Windows penetration testing home lab but decided that it could be more useful running a Unix based operating system. I narrowed down my search to a Linux operating system, but this came with a tough decision in the decision process. I narrowed down my search to a Linux operating system, but this came with a tough part in the search. There are many different types of Linux distributions, from the famous Kali Linux to Ubuntu, Xubuntu, Debian, and many more! I initially installed Fedora 12 on the machine with the XFCE environment, and it worked well for a bit. Ultimately, I switched from Fedora 12 and opted for a Debian-based distribution called  [Pop!_OS](https://system76.com/pop/), which has a great reputation for being compatible with older machines.

**Step 2: Purchasing hardware upgrades:**

The battery works surprisingly well for being dormant for two years and being heavily used from 2014 to 2022. However, other aspects **needed** to be changed in order for the machine to be actually useful. The first item that had to go was the default 1000GB HDD. The hard disk was simply to slow and not ideal for our needs. I swapped it out for a 500GB Solid State Drive on Amazon.com that just cost me $30 and the machine boots up fast than I have ever seen it before. In addition to the SSD, I also installed 16GB of DDR3 RAM which is the maximum amount of RAM that Lenovo supports for this laptop. Back when I got this laptop, 16GB of DDR3 would have cost me over 100 dollars but nowadays it only costs about $18 dollars.

**Step 3: Installing new drivers:**

The laptop was now up and running with a fantastic operating system and new solid state driver along with RAM. The next part revolved around getting the drivers installed. To my amazement, PopOS had a lot of drivers already installed and ready to go.

**Step 4: Making compromises**

One area that I had a challenge with regarding this laptop was getting the dual Nvidia/Intel graphics to work properly on it. The Lenovo Y50–70 has a Nvidia 860M graphics card built into it and it also has a Integrated Intel Chip. Unfortunately, I was not able to get the Nvidia 860M graphics card to work and so the gaming days for this laptop are most likely over. However, I am alright with that as it will serve it’s purpose now as a component of my homelab. In addition, the monitor on the laptop is not the best at default and could be upgraded but I am holding off on this for now as new monitors are quite expensive and I am not willing to invest 70 dollars on a new monitor for the laptop when I could just attach an external monitor.

**Step 5: Next step**

I’m not sure what exactly I will run on the laptop but I am leaning towards installing the Damn Vulnerable Web Application(DVWA) for penetration testing practice. Stay tuned for my write-up on the first project that I use with this laptop very soon!