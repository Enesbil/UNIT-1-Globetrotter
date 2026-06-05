What location are you building this guide for, and why did you choose it? Istanbul, its an attractive location and I know a lot about it being from there.
Who is your primary audience? (e.g., first-time visitors, backpackers, families, local residents)
Gen Z Western/USA audience, first time visit lead. I knowistanbul enough and i know the western context enough putting me in an adventagous position. Also Istanbul prolly wants to attract more western tourists anyways so it would be the city's goal too.
What do you want visitors to feel or know after spending 5 minutes on your site? Curiosity, and a new positive/positiver attitude towards the city.
What's one design decision (color, layout, or tone) that reflects your destination's identity?
Look at my thoughts section below. Example is color scheme choices with the bordeaux which is a notable color in turkish culutre/history


My thoughts 
- Modern but not out of touch with the culture -- Accurate to Gen Z target
- Color scheme should reflect above philosphy, smtn with light bordeaux as one of the main colors but keep it modern 
- Nice stretch goal would be like adding embroidery/turkish art style css border components - can use ai for this 
- Inspo sources: https://www.visiticeland.com/, https://goturkiye.com/, 
- I'm thinking like a neobrutalist style. if theres a good skill for it use it maybe
- Create design spec first 
- use big images 

pt 2
use grid for the image galleries
have some variety on layour styles across var pages
do things that actually reflect the city
get rid of all the em dashes

pt 3 
go over all the code and actually understand fully
deploy via render
reduce animations and simplify on smaller screen sizes
write the documentation


---
build plan (filling this in as I go)

pages im building:
- Home: the split Europe / Asia hero, the ferry fact stripe, two feature blocks, and a where next section at the bottom
- Top Attractions: Hagia Sophia, Blue Mosque, and the Grand Bazaar, each with a number, a photo, and a writeup, plus a map at the end
- Eat: my food guide, three spots (breakfast, midday, dinner) each with an address, description, and a menu link
- Cattractions: the cat photo gallery, masonry style, every photo has a caption

layout approach:
- flexbox for the nav, hero, footer, and the button rows
- grid for the attractions and the home features so the pages dont all feel identical
- everything collapses to one column on mobile

responsive plan:
- hamburger nav on phones, kept it CSS only so no JS
- reorder the grid cells on mobile so each image sits right above its own text
- simplify and cut down the animations on smaller screens like I noted up in pt 3

still to do:
- deploy on render
- record the walkthrough video
- one final pass over all the code so I actually get every part of it
