# Bitty Buddies Archipelago
(This is the standalone repository for the Bitty Buddies APworld.
If you're looking for the corresponding fork of the main archipelago repository, you can find it
[here](https://github.com/bmorledge-hampton19/Archipelago/tree/bitty_buddies))

## What is Bitty Buddies?

Bitty Buddies is a short, genre-spanning experience and a love letter to retro handheld gaming. Dust off your Bitty
Boy and slot in one of your 5 favorite cartridges, each containing a unique game to chase high scores in. As your
scores improve, you'll unlock and level up the "buddies" that call each cartridge home. Each of them is proficient
in their own game, but with some experimentation, you'll find that their true talent lies elsewhere...

## Where can I play Bitty Buddies?

You can play Bitty Buddies for free at https://mr-dr-bean.itch.io/bitty-buddies. The game can be played in-browser
(even on a mobile device), or you can download it for Windows, MacOS, or Linux.

## How do I install the Bitty Buddies APworld?

First, make sure that you have downloaded the latest
[Archipelago release](https://github.com/ArchipelagoMW/Archipelago/releases/latest).
Then, download bitty_buddies.apworld from the
[latest release](https://github.com/bmorledge-hampton19/bitty_buddies_apworld/releases/latest)
and copy it into the /custom_worlds directory in your local archipelago folder.

## How do I create a config (yaml) file for this game?

If you're familiar with editing yaml files by hand, you can use the "Bitty Buddies.yaml" file from the
[latest release](https://github.com/bmorledge-hampton19/bitty_buddies_apworld/releases/latest) to use as a template.
Otherwise, you can use the Options Creator in the Archipelago Launcher for a more straight-forward interface.
(This will only work if you have already installed the Bitty Buddies APWorld.)

## How do I join an Archipelago multiworld with Bitty Buddies?

If this is your first time running an archipelago randomizer, you can find lots of helpful
information about the process in the [Archipelago Setup Guide](https://archipelago.gg/tutorial/Archipelago/setup_en)

Once you've generated a Bitty Buddies settings file (.yaml) and have it hosted somewhere, you should be able
to connect to your slot from directly within the game.
Start Bitty Buddies, and from the main menu, select "Randomizer" to switch to the randomizer's main menu.
From there, select "Archipelago" and enter the server address, your slot name, and (optionally) your password to connect.
That's it! The archipelago saves independently from the base game or local randomizer,
so your high scores will persist if you lose connection. You can even have multiple players join the same slot
for cooperative play, and progress should sync between everyone automatically.

## What does randomization do to this game?

Buddy level ups, cartridge-specific bonus points, and optionally, buddy power increases, are randomized into the item pool, and random items are sent
when you achieve goal scores in each cartridge or fulfill special "silly" or "skill" checks (see below).
The buddy that you start with will also be randomized.

The gameplay itself is unchanged, but you may find yourself forced to develop new strategies as you play through the
game with a different lineup of buddies than you're used to!

## What's the goal?

The goal is to achieve the total high score specified in your YAML. The default goal score is 999 (the same as the
base game) but you can set it as high as 2000 points if you're looking for a challenge!

## How do I track my progress during the randomizer?

All of the your progress in the randomizer can be tracked in-game. The check marks below each buddy icon on the
Bitty Boy represent the number of goal scores you have achieved in that buddy's cartridge. Also, remember that you
will receive additional checks when you have achieved the first, second, third, and fourth goal scores across ALL
cartridges (the "buddy power" checks). If you have silly and/or skill checks enabled, these will be represented
by unique symbols below each buddy's goal score check marks.

When you are selecting a game to play from the main Bitty Buddies cartridge, both your current high score and
the maximum score in logic will be displayed. If the logic score is higher than a goal score that you have not
yet achieved, it will be suffixed with an exclamation point! (This exclamation point will also show up when
you have a silly/skill check in logic for that cartridge.)

## What are the "Silly Checks" that can be enabled in the options?

The silly checks are 5 extra tasks for buddies in their sub-optimal cartridges:
- Bud's silly check (Mean Mugging): Get your shoe stolen by an angry balloon in Bazz's Big Day.
- Biff's silly check (Heavyweight Champion): Drop to the ground without slowing your fall in Acrobird.
- Benson's silly check (Frictionless Fruit): Hit one of the banana peels with your tire in Trash Dash.
- Brie's silly check (Negative Jing): Have Brie fly away from Have at Thee by refusing to block or attack.
- Bazz's silly check (0-Star Review): Pop the tires on a customer's car by getting too close in Treatment To-Go.

## What are the "Skill Checks" that can be enabled in the options?

The skill checks are 5 extra tasks for buddies in their optimal cartridges:
- Bud's skill check (Fast Pharma): Deliver orders to three different customers within 7 seconds in Treatment To-Go.
- Biff's skill check (Parry King): Deflect 5 balloons with a single block action in Bazz's Big Day.
- Benson's skill check (Miracle Cure): Go below 0 hp and survive by regenerating health in Have at Thee.
- Brie's skill check (High Flyer): Fly over a paper airplane in Trash Dash.
- Bazz's skill check (Sharpshooter): Score a bullseye on a small, moving target in Acrobird.

## How does death link work in this game?

Death links are sent when you receive a game over in a cartridge without at least matching your previous high score.
This also applies to games you end manually (via the pause menu), so be careful about needlessly resetting!

Received death links can have one of two different effects, based on your settings:
- Game Over: Death links trigger a game over.
- Next Buddy: Death links trigger a transition to the next available buddy (as if the current buddy just failed).

Additionally, when you receive a death link, the affected attempt becomes exempt from sending a death link.
