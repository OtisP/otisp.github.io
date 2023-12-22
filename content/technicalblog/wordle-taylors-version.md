+++
title = "Wordle (Taylors Version)"
date = "2023-12-17T14:18:04-05:00"
draft = false
#
# Set menu to "main" to add this page to
# the main menu on top of the page
#
#
# description is optional
#
description = "Wordle (Taylor's Version) is a Wordle inspired word game where users attempt to guess a Taylor Swift song given a portion of the lyrics"

#
# tags are optional
#
# tags = []
+++

# Wordle (Taylor's Version)
Quick blog post for a project that was almost done about a year ago, but decided to push it through so that I could make a blog post.

#### Important Links

- Download the app! (Coming soon!)
- Check out the [code](https://github.com/OtisP/Wordle-Taylors-Version)
- [Tell me](mailto:wordle@otispeterson.com) you like (or don't) the game!

## What is it?
Remember Wordle? The fad from 3 (😬) years ago now? What if you had to guess a Taylor Swift song based on lyrics instead. This *sort* of thing has been done, with [lyricle](https://www.lyricle.app/), and the [lyricdle](https://www.lyricdle.app/), and the [taylordle](https://taylordle.org/), and I'm sure more... but never before has someone executed this exact combination of an idea!

### So how do you play?
Every day a random Taylor Swift song is chosen[^1] and 6 random lines from that song are chosen.  There's a basic check to make sure the song title isn't explicitly revealed in the lyrics of the song. And then you get 6 guesses! For every guess, if the album is correct then that guess will be marked yellow, and if you get the correct song and album your guess is marked green and you win 🙌.
 
### Sounds like you need to know a lot about Taylor Swift songs
Definitely. This is much more of niche game that (despite how many swifties there are) is unlikely to find a seriously wide appeal.


### Is it just as fun as Wordle?
Whoa you're getting kinda judgy there. The original Wordle™ has a genius simplicity of giving you 5 pieces of information for every guess - one for every letter. Other song related "dle"s have struggled with a similar issue I did here, the user only really inputs 2 pieces of information for every guess: the song and the album. This seriously hurts the games potential, but nevertheless we push on.


## How did you make it?
The biggest resource that I got to leverage was a compiled list of the lyrics in an easy to use form. A fellow swiftie has [automated](https://github.com/shaynak/taylor-swift-lyrics) this process for the purposes of making a Taylor Swift [Lyric Search](https://shaynak.github.io/taylor-swift/). I downloaded the csv directly and made some manual edits to make the data a little prettier for what I needed it for. Aside from that, the UI built using pretty standard SwiftUI. I tried to adhere generally to an MVVM structure, but I wrote most of this code over a year ago when I was only 6 months into learning Swift. I could refactor it all but I kind of like this as a timestamp of my abilities. Proof of \*\~growth\~\*. 

The code is open source and can be found [here](https://github.com/OtisP/Wordle-Taylors-Version).


### What did you leave out?
There were lots of vague feature ideas that got cut so that I could get an MVP published. Some include:
- Keeping stats for all past guesses
- An explanation of the rules (eek)
- Keeping track of a "streak" to encourage people to play it consistently
- Comprehensive testing

Open to other ideas! No promises on implementation but feel free to [reach out](mailto:wordle@otispeterson.com), or even open a [pull request](https://github.com/OtisP/Wordle-Taylors-Version/pulls) if you feel so inspired. I can update this list as features get suggested/rolled out.

### Biggest shortcoming?
I don't have that much design experience, so every decision is made on gut feeling which can lead to some, less than ideal colors/shapes. Working in industry has definitely lead to a reliance on a designer handing me a mock of the final product and working backwards from there. Again, a skill I will no doubt improve at the more I try.

## Final thoughts

Here's a screenshot of the game! You've earned it. 
![screenshot](/images/wordle_screenshot.png)

I love a silly little word game. Thought I'd try my hand at making my own and meanwhile practice some iOS development from the ground up, all in all, a rousing success 😄.

I'm also obviously a Swiftie, I got to see her in Philly, night one. My favorite album is Speak Now, but I'm in my folklore era.

In case you also like silly little word games, please enjoy my silly/serious little word game list I do on a daily(ish) cadence:
- [NYT Crossword](https://www.nytimes.com/crosswords)
- [Connections](https://www.nytimes.com/games/connections)
- [Waffle](https://wafflegame.net/)
- [Quordle](https://www.merriam-webster.com/games/quordle/#/)
- [Anigrams](https://anigrams.us/)[^2]
- [Puzzmo](https://www.puzzmo.com/today) holds various word games inside
- And of course: [Wordle](https://www.nytimes.com/games/wordle/index.html)





[^1]: I limited this to her 10 main albums, plus the holiday album. We don't need to think too hard about songs like [Macavity](https://www.youtube.com/watch?v=_KYkIhqrXGQ) (And technically I left in "I heart ?" but I had to)

[^2]: Developed by various folk in the crossword community!
