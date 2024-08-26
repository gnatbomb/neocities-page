# Klepto-Chronia

<iframe width="100%" height="350" src="https://www.youtube.com/embed/hGhe1ZRktAc" title="Klepto-Chronia Trailer" name="Trailer" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>Trailer</iframe>

Play as Amelia, a time-travelling ~~thief~~ archeologist from the future, who is trapped in the past. Freeze time to sneak past robot guards in this 2d stealth-puzzler, as you explore the mansion of the reclusive genius Dr. Ology, and try to find a way home.

### [Click here to play!](/Gold/www/index.html)
 
This game was made over a period of four months as part of the University of Alberta's CMPUT 250 Game Development course. I composed the soundtrack, handled all in-game sounds, helped with the programming and writing, developed most of the puzzles, and led my team as the producer. I also handled user testing, and provided actionable feedback to my team based on that testing.

Klepto-Chronia was awarded the CMPUT 250 Game of the Year award.

[You can stream or download the soundtrack here!](https://nataliebombardieri.bandcamp.com/releases)

# Dynamic Soundtrack

When the player freezes time, the game music is softened and a clock's "tick-tock" sound can be heard.

The idea that I had in mind was to tie the game's music to the player's time-stasis ability, in order to make the main game mechanic feel impactful, and clarify to the player whether or not they have time-stasis activated. 

I tested the idea in earlier builds by simply changing the volume of the music, and playing a ticking sound effect at a set interval. This was noticed and appreciated by testers, but raised a number of technical problems that made it negatively affect gameplay, as well as producing unsatisfactory results.

I instead decided on an approach that involved having two versions of each song in the game, with one having different audio mixing and a "tick-tock" sound overlayed and lined up to the beat. 

This removed the need to have an in-game timer running in the background, which checked every half-second if we needed to play a tick or tock sound effect; something that the game engine we were using did not handle well.

Adding the ticking to the track directly also had the added benefit of ensuring that the ticking would line up to the beat of the song, as before it may have been slightly off due to load times not lining up.

Finally, having two versions of each song allowed me more control over sound, as now I could change the audio mixing instead of only being able to control the volume of the song.

For creating the "tick-tock" versions of each song, I used a few after-effects that I plugged all of the instrument tracks into, which dampened the sound (reduced the volume for higher frequencies more than for lower frequencies), and added a slight amount of reverb, which made it sound like the music was coming through a wall. I could turn these effects on and off to quickly switch between versions of the song, while sharing the same notes and rhythms otherwise.

Having this at my disposal made it simple to change and update the music, without having to make duplicate changes in multiple places, which saved me a lot of time while I was writing (and rewriting, and rewriting) the music.

Lastly, I used [Jay's Variable Mix BGM Manager](https://forums.rpgmakerweb.com/index.php?threads/jays-variable-mix-bgm-manager-version-1-0-2.58373/) to allow me to switch between track versions seamlessly, by fading in the new track over half a second so that the transition is smooth.


# Consistent Climax Music Timing

During the final in-game cutscene where the Amelia confronts Dr. Ology, the music seamlessly progresses and increases in intensity, while accounting for different reading speeds for the player. 

[Listen to the song here!](https://nataliebombardieri.bandcamp.com/track/apologies-finale)

Having wanted to create an emotionally engaging climax, I wrote a song that plays during the climax, and grows in intensity to match the tone of the dialogue in the cutscene.

However, something that I noticed during testing was that for varying reasons, playtesters progressed through the climax dialogue at widely different speeds. For some players, this meant finishing the climax dialogue before the music could get intense. For other players, it meant that while they read, the music would grow in intensity too soon, and would have no music while they reached the climax.

My solution to this issue was to split my finale song into six parts, and use the plugin mentioned above to switch to the next part as the player reached certain points in the dialogue. The music would loop portions of the song if a player was reading slowly, and grow in intensity at the right moments, ultimately swelling and climaxing alongside the high-point in the plot. Players who read faster were accomodated for by transitioning sooner to more intense parts of the song.

This approach allowed players to receive a consistent audio experience every time, regardless of how long they took to progress the dialogue.









<!---[![Klepto-Chronia](https://raw.githubusercontent.com/gnatbomb/gnatbomb.github.io/main/kleptotitle.png?token=GHSAT0AAAAAABTO7NESM64CWSLVIPXUCHKKYT5R4UA)](https://gnatbomb.github.io/)


[![Klepto-Chronia-Title](https://raw.githubusercontent.com/gnatbomb/gnatbomb.github.io/main/kleptotitle.png?token=GHSAT0AAAAAABTO7NESOSYUPNGSC5SOV7D4YT5PI3A)](/Gold/www/index.html)
 
## [Gold Release - Click here to play!](/Gold/www/index.html)

## [Trailer](https://www.youtube.com/watch?v=hGhe1ZRktAc)
<iframe width="560" height="315" src="https://www.youtube.com/embed/hGhe1ZRktAc" title="Klepto-Chronia Trailer" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

I wrote the soundtrack, which is available for download or streaming here: [Bandcamp](https://nataliebombardieri.bandcamp.com/releases)

### Controls

WASD - Move

Enter - Interact with world objects / Progress dialogue

Space Bar - Time stasis

Esc - Menu

Mouse - Progress Dialogue / Hold to fast-forward Dialogue
 
### Gameplay

In Klepto-Chronia, you play as Amelia, a time travelling ~~thief~~ archeologist from the future, as she visits the past to ~~steal~~ recover artifacts  before they are lost to time.

When Amelia's time-hacker breaks mid ~~heist~~ expedition, she has to solve puzzles while avoiding being caught, in order to make her way through the mansion of Dr. Ology, and find her way home.

Amelia's broken time device can freeze time in a small area around her, allowing you to temporarily disable guard robots, pressure plate functionality, and door movement.

Klepto-Chronia was made in Winter 2022 for the CMPUT 250 Games Development course at the University of Alberta.


### Friendly Skeleton Games 

- Natalie Bombardieri	
    - Producer, Audio, Programmer, Writer
- Mason Bly	
    - Programmer, Lead Designer
- Bailey Danyluk	
    - Programmer
- Leslie Quin	
    - Programmer
- Cassandra MacCarthy	
    - Writer
- Alec Zaiane	
    - Artist
- Lisa Bourque	
    - Executive Producer

### Gold Release
[Web](/Gold/www/index.html)
 

### Stream or download the Soundtrack!
[Bandcamp](https://nataliebombardieri.bandcamp.com/releases)
 
 
## Beta versions of the game

### Beta 2: the sequel

[Web](/Beta2/www/index.html)
 
### Beta 
 
[Web](/BetaWeb/www/index.html)


### Vertical Slice (Old)
 
[Web](/VS/GameFiles/www/index.html)
 
 
### Barebones Tech Demo (Old)

[Web](/TechDemo/index.html)--->

 

