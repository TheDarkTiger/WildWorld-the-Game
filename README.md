# Wild world simulator
![screenshot](doc/screen.png)

## Basic info:
- Game written in OOP Python.
- GUI made in tkinter library.
- PEP8 standard used (mostly) for easier code reading and editing.
- Was 'micmarty' very first Python project.

## How to run
1. Make sure you have **Python** installed(version 3 is preffered -> I tested it on 3.5.2 and it worked like a charm)
2. Install **tkinter** library
```
$ sudo apt install python3-tk
```
3. Type in terminal/console:
```
$ python3 World.py
```


## ~~Rules~~
no rules, it's a sandbox or a simulation
1. There are 9 creatures.
2. Each one has its own attributes, like: 
  - initiative - decides who moves first
```
example: Fox is smarter, so he moves first, then Turtle, etc.
```
  - strength - the stronger the animal is, the more enemies it can defeat
  - age - if there are two animals with the same initiative, older one moves first.

**what animal species does:**
  they move around, reproduce themselves, kill each other and eat plants

**what plants does**
  they just spread around the map and make no moves


## Animals:
Spiecies | icon | desciption | strength | initiative 
------ | ------ | -------------|-------------|---------------
Human | ![human_icon](icons/czlowiek.png) |  he moves using WSAD, drink stamina elixir - that gives up to 10 strength on 'T' key press, in game he is a 'C' letter, like "człowiek" in polish | - | -
Wolf | ![wolf_icon](icons/wolf.png) | - | 9 | 5
Sheep | ![sheep_icon](icons/owca.png) | - | 4 | 4
Fox | ![fox_icon](icons/lis.png) | SMART power: fox never goes on stronger enemy's teritory | 3 | 7
Turtle | ![turtle_icon](icons/zolw.png) | <ul><li>MOTIONLESS power: turtle has lower chance to move somewhere. Often stays in place.</li><li>>SPARTAN SHIELD power: turtles can avoid enemies which have less than 5 points of strength</li></ul> | 2 | 1
Antelope | ![antelope_icon](icons/antylopa.png) |  <ul><li>CRAZY JUMP power: antelope jumps every 2 fiels instead of 1(like other species)</li><li>FAST ESCAPE power: antelope has a 50% chance to do an additional move during a life threatening situation</li> | 4 | 4

## Plants:
Plant | icon | desciption 
------- | ----- | -------------
Grass | ![grass_icon](icons/trawa.png) | just grows, useless
Sow thistle | ![sow_thistle_icon](icons/mlecz.png) | takes 3 attempts to spread somewhere
Guarana | ![guarana_icon](icons/guarana.png) | once eaten gives +3 strength
Deadly nightshade | ![deadly_nightshade_icon](icons/wilczajagoda.png) | kills if eaten

## Additional features:
- You can SAVE game into file (txt), and then LOAD it
- There are 2 boxes, that informs you about events (killing, eating, reproducing)
- You don't need to click 'NextRound' button, just press ENTER
- MAGIC PEN, hover with mouse at some field. Randomly generated organism will appear.

## TODO
- [ ] adapt to new PEP rules
- [ ] review old code to clean it up
- [ ] review the interface to make it more attractive
- [ ] add a timer to make the game step automatically
- [ ] rename icons from polish to english
- [ ] maybe use PyGame




