---
layout: post
title:      "My First CLI Gem - Game_Of_Thrones"
date:       2019-05-14 02:26:05 +0000
permalink:  my_first_cli_gem_-_game_of_thrones
---


Just a few months ago the extent of my coding knowledge was a couple of basic tutorials that I had worked through on different coding sites.  I've been working in digital marketing for a few years now and looking at the back end of a website, I had no idea what any of the code said, but I thought it looked interesting and I wanted to learn how to read it.  I started attending the Flatiron School back in March and my cohort just finished up our Object-Oriented Ruby portion of the curriculum.

At the end of the Object-Oriented Ruby section of the class, we were tasked with building out our own CLI gem.  I decided that I would build a scraper to scrape imdb.com and pull in the titles of Game Of Thrones episodes.  This project was very challenging for me since it was the first time that I built a program from scratch, but it was super exciting when I finished it.

Before I began the project, I went through some of the old labs and watched Avi Flombaum's [CLI Gem Walkthrough](https://www.youtube.com/watch?v=_lDExWIhYKI) video.  He did a great job at explaining the steps and after watching the walkthrough, I was ready to begin building out my gem.

I first created the gem using "bundler gem" in my Learn in-browser IDE.  I then pushed that gem to Github and made sure it was all set up correctly.  Next, I had to add an executable file `!/usr/bin/env ruby` so that I could run the program.

I started to stub out my CLI and added some methods with if/else statements and case statements to make sure that the CLI worked.  I wanted to get the shell of my program working before I started building the scraper method.  I got this up and running and pushed it to Github.

One of the biggest things that I would do differently next time is to write more meaningful commit messages.  I'm not sure if my internet was acting up or if the Learn in-browser IDE was acting up but unfortunately I got disconnected a few times and lost some code.  After this, I was pushing changes to Github with less than meaningful commit messages every time I made a few changes to the code.

The thing that took me the longest when building out my gem was figuring out how to scrape the information from the page.  I originally wanted to use a Wikipedia page but I couldn't figure out how I needed to scrape the information.  I moved on to Imdb.com and was able to pull the episode name for each season.

Now I had a working program that was scraping data from a specific website.  I thought I was done so I started testing my program and noticed that I was storing the episode names in an array but not clearing that array when I went back to get the episode names from a new season.  I thought about how to correct this and decided that I would add a line of code, `Game_Of_Thrones::Episodes.destroy_all` to clear the array each time the episodes were listed.

My CLI gem was now complete, but there are still things that I would like to go back and add to it.  I want to add a choice to select more information about each episode from each season and return back episode descriptions and the date that the episode first aired.  Maybe I could also find a website that has additional information about specific episodes, possibly meaningful quotes, characters who were killed in the episode, interesting facts, etc.

Building my first CLI gem was definitely a challenge, but in the end I did something that just a few months ago I couldn't dream of completing.  I can't wait until my next big project.
