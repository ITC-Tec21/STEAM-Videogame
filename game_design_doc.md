# Circuit Sandbox
> Game Design Document
> Sebastian Juncos
> Agustin Pumarejo
> Adriana Abella
# Table of Content

- [Game Design](#game-design)
    - [Summary](#summary)
    - [Gameplay](#gameplay)
    - [Mindset](#mindset)
- [Technical](#technical)
    - [Screens](#screens)
    - [Controls](#controls)
    - [Mechanics](#mechanics)
- [Level Design](#level-design)
    - [Themes](#themes)
    - [Game Flow](#game-flow)
- [Development](#development)
    - [Abstract Classes / Components](#abstract-classes--components)
    - [Derived Classes / Component Compositions](#derived-classes--component-compositions)
- [Graphics](#graphics)
    - [Style Attributes](#style-attributes)
    - [Graphics Needed](#graphics-needed)
- [Sounds/Music](#soundsmusic)
    - [Style Attributes](#style-attributes-1)
    - [Sounds Needed](#sounds-needed)
    - [Music Needed](#music-needed)
- [Schedule](#schedule)



# Game Design

## Summary
A puzzle/simulator game in which the player has to partially or completely build a circuit using logic gates given a circuit specification. 

## Gameplay
The player will drag and drop components to edit the circuit. The number of movements/components used to complete the circuit will determine the player's score for that level (less movements/components = higher score). Players can toggle a real-time visual simulation of the circuit. 


## Mindset
Players will feel like each level is challenging, but still within their understanding. As they progress, they will develop their own strategies and begin to recognize patterns in the circuits. In the latest stages of the game, the players will feel confident when approaching a new level and also eager to find challenging puzzles.
Due to the fact that score isn't calculated by the time it takes for you to complete the level but rather the number of movements, the player will feel calm and at the same time concentrated and invested in what they're doing.

# Technical
In order for the game to simulate and verify circuits accurately, each one of them will be represented as a map in the following way:
- Nodes = logic gates
- Edges = wires
- Leaves = inputs
- Root = output
 
## Screens

1. Title screen
	a. Options
	b. User score
	c. Credits
2. Level select
3. Game
	a. Pause
	b. Gate select
	c. Circuit

## Controls
The player will drag and drop logic gates into and out of the circuit to modify it. 

## Mechanics
Each level will replicate a real-life functioning circuit. The circuits are dynamic and they change in real-time when the player interacts with them.
Are there any interesting mechanics? If so, how are you going to accomplish them? Physics, 
algorithms, etc.

# Level Design 
1. Tutorials: There will be no circuits to edit, you'll only be able to interact with a single logic gate at a time in order to understad the way it works.
2. Basic levels: There will be a small amount of inputs and outputs and each level might have many distinct solutions.
3. Intermediate levels: The size of the circuits will be increased, only a few combinations will result in the correct output, and you're introduced to a wider variety of logic gates.
4. Advanced levels: There will be only one or two distinct solutions and more logic gate types to work with and the player will have to work towards more precise circuit specifications.

## Themes
1. Mother board circuit
2. Individual circuits
3. 
## Game Flow
1. Tutorials
	a. Logic gate
		i. A circuit with 2 inputs, a logic gate and 1 output is presented to the player
		ii. The player changes the inputs of the circuit to learn how that logic gate works
		iii. When the player is comfortable and understands the logic gate, they move to the next section
	b. Circuit introduction
		i. A slightly more complex circuit is presented to the player
		ii. All of the components are explained to the player
		iii. The player can change the inputs or logic gates to learn how a circuit works
	c. Important concepts explanations
		i. Circuit specifications
		ii. Truth tables
		iii. Circuit comparison with natural language
2. Circuit completing levels
	a. A circuit with fixed input values and no logic gates is introduced to the player
	b. The player reads the level's objective
	c. The player uses the logic gates available to complete the circuit and achieve the objective
	d. The player submits their solution
	e. The solution is tested by the game
	f. If the solution is correct, the player moves on to the next level. If not, they can keep trying.
3. Circuit repairing levels
	a. A circuit with changeable input values and no logic gates is introduced to the player
	b. The player reads the level's objective, which consists in repairing the circuit so that it meets its given specifications
	c. The player uses the logic gates available to complete the circuit and achieve the objective, changing the input values to test their solution
	d. The player submits their solution
	e. The solution is tested by the game
	f. If the solution is correct, the player moves on to the next level. If not, they can keep trying.

# Development
 
## Abstract Classes / Components
1. BaseLogicGate
2. BaseInput
3. Output
4. Wire
5. InteractableButton
6. InstructionsUI
7. GatesUI
8. GameManager
9. MainCamera

## Derived Classes / Component Compositions
1. BaseLogicGate
	a. AND
	b. OR
	c. NOT
	d. NAND
	e. NOR
	f. XOR
	g. XNOR
2. BaseInput
	a. FixedInput
	b. ChangeableInput
3. InteractableButton
	a. HomeButton
	b. SettingsButton

# Graphics

## Style Attributes
- Simple solid art style
- Dark-themed
- Dark blue and white color palette
- Green or red inputs/outputs

## Graphics Needed
1. Logic gates
	a. AND
	b. OR
	c. NOT
	d. NAND
	e. NOR
	f. XOR
	g. XNOR
2. Inputs
3. Outputs
4. Wires
5. Buttons
	a. Start button
	b. Home button
	c. Settings button
	d. Level select button
	e. Credits button
	f. Next section button
	g. Instructions button
	h. Logic gates button
6. Logic Gates UI
7. Instructions UI
8. Background

# Sounds/Music
 
## Style Attributes
Music:
- Futuristic
- Lo-fi
- Electronic instruments
- Shepherd effect
- Ten-minute loops

Sound effects:
- Clean
- Star wars like

## Sounds Needed
1. Effects
	a. Logic gate dropped
	b. Input changed
2. Feedback
	a. Wrong solution sound
	b. Correct solution sound

## Music Needed
1. Chill ambient sound "main menu" track
2. Medium-paced synth arpegios music "level" track

# Schedule
 1. Define style and gameplay
 	a. Base style 
		i. Logic gates
		ii. Bakcground
		ii. Mechanics
2. Create main assets 
	a. Base level components
		i. All logic gates
		ii. All cables
		iii. Inputs and outputs
		iv. Game tools
	b. Base GUI components
		i. Menu buttons
		ii. Settings buttons
		iii. Volume Settings
3. Level Design
	a. Define Logic gates for each level
	b. Check difficulty of each level so that they are balanced
4. Design music
5. Design effects
