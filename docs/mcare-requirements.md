# WHO Mass Casualty AR Experience (MCARE) Game Simulation

## Engineering Requirements

## Summary

The purpose of this serious game is to save lives by training hospital staff to avoid being overwhelmed by the cognitive and physical load associated with a mass casualty event. MCAR is immersive, on-demand collaborative learning experience for a worldwide audience. The game enables healthcare teams to increase local hospital capacity and speed response to a mass casualty event by training in a simulation matching local conditions and resources. 

A LIDAR 360-degree camera maps each hospital’s emergency care areas to present in augmented reality. Gamification increases engagement. Teams increase their scores by improving patient flow and management. Scoring is computed based on patients’ Minutes of Life, as increased by players taking correct decisions and actions. Multiple simulation modes from realistic to high challenge use an intuitive interface and a low-cost deployment strategy. Attractive user interface is easy to use with hand navigation. 

## Source Code License

MIT Open Source. Hosting on Github.

## * 1\. Hardware
   * 1.1 Magic Leap One
   * 1.2 Microsoft Hololens 2
   * 1.3 Slamtec RPLIDAR M1M1 Lidar 
   * Insta360 One X2 360-degree camera
   * 1.4 On-prem server

## * 2\. Software
  * 2.1 WebGL
  * 2.2 WebXR
  * 2.3 A-Frame
  * 2.4 PHP
  * 2.5 SQL

## * 3\. System Capabilities
  * 3.1 3D
  * 3.2 Gesture
  * 3.3 Gaze
  * 3.4 Speech recognition
  * 3.5 Dictation
  * 3.6 Remote pointer
  * 3.7 Remote assistance
  * 3.8 Checklists
  * 3.9 Playback
  * 3.10 Rejoin
  * 3.11 Lobby
  * 3.12 Snapshot
  * 3.13 Pause, Stop, Play
  * 3.14 Auto-save
  * 3.15 Barge-in
  * 3.16 HUD

## * 4\. Simulation Features
  * 4.1 A user to run a simulation
  * 4.2 Repeat the simulation 
  * 4.3 Monitor progress 
  * 4.4 Restart to attempt new strategies
  * 4.5 Save feedback
  * 4.6 Pseudo-randomized presentation of different numbers of patients entering the ER after a mass casualty event
  * 4.7 A specific Life Path for each virtual patient
  * 4.8 Points scored based on increasing the total number of minutes of life added to each patient
  * 4.9 A patient who undergoes several stages of complication will have scores assigned to the management of each phase
  * 4.10 A fair die roll probability give Hits for treatment success
  * 4.11 Increased challenge difficulty in response to achieving good results
  * 4.12 Leaderboard
  * 4.13 Self-authoring, in that new content can be continuously uploaded
  * 4.14 Directed play, responsive training that when specific types of simulation conditions overwhelm the response team, more practice at that element is provided
  * 4.15 Simulation intensity setting can be adjusted with respect to severity of cases, numbers of cases managed per unit time and through gradually being able to admit more and more patients in a tight time window and improve outcomes
  * 4.16 Redo, permit the team to return to identical conditions for later play

## * 5\. Game Modes
  * 5.1 Walk-through: users familiarize themselves with the simulated environment and learn the game features
  * 5.2 Free-form: simulator interface to increase patients per time, the types of patients that arrive and other conditions such as number of doctors, nurses or available beds
  * 5.3 Gaming: teams take on increasingly more difficult conditions with the opportunity to freeze game progress and communicate about solutions, real-time through the game interface
  * 5.4 Overload: game intensifies conditions until the team fails according to defined criteria
  * 5.5 On-demand: instructor adds new cases to the simulation set when a team is struggling with a particular type of case

## * 6\. Game Characters
   * 6.1 Incident Commander
      * 6.1.1 This character can ??? *Recommendation: they can do some shared activities as the others can do (move, answer questions, treat patients?), but they have access to an indicator that shows #of beds available, #of patients in green/red, #of patients needing immediate attention, can send doctors/nurses to different zones. I need JJ to provide me with more context on each of the roles.*
   * 6.2 Clinical Lead
      * 6.2.1 This character can ??? *Recommendation: they can do some shared activities as the others can do, but they have access to an indicator that shows #of patients in green/red, #of patients needing immediate attention, can send doctors/nurses to different zones??.*
   * 6.3 Resource Lead
      * 6.3.1 This character can ???? *Recommendation: they can do some shared activities as the others can do, but they have access to an indicator that shows #of beds, # of different equipment, ??.*
   * 6.4 Triage Officer (says if a patient is walking or non-walking)
      * 6.4.1 Decide whether to direct new patient to red or green zone. Anything else?
   * 6.5 Red Zone #1 Emergency Responder
      * 6.5.1 This character can ??? *Recommendation: they can do some shared activities as the others can do, but they have access to an indicator that shows #of patients in red, #of patients needing immediate attention, can send someone to the green zone??.*
   * 6.6 Red Zone #2 Emergency Responder (team, minimum 2 players)
      * 6.6.1 This character can ??? *Recommendation: they can do the same as Red Zone #1 but when they work together successfully, they earn some type of bonus together.   
   * 6.7 Green Zone #1 Emergency Responder
      * 6.7.1 This character can ???? *Recommendation: they can do some shared activities as the others can do, but they have access to an indicator that shows #of patients in green, #of patients needing immediate attention, can send someone to the red zone??.
   * 6.8 Green Zone #2 Emergency Responder (team, minimum 2 players)
      * 6.8.1 This character can ??? *Recommendation: they can do the same as Green Zone #1 but when they work together successfully, they earn some type of bonus together. 

Any character may be a player or NPC (Non-Playable Character, a bot). The game may play entirely against itself using AI to create hospital simulations. All players/NPCs have avatars.

## * 7\. Gameplay
   * 7.1 "Command and Conquer” mechanics for selection and movement of "virtual staff”. Group selection and dropzone with hand movement. https://www.ea.com/games/command-and-conquer 
   * 7.2 “Diving" into a room when patient treatment is required. More than one person may dive into the room. Some procedures require 2 people to agree on them.
   * 7.3 A large virtual panel with procedures is displayed when diving into a room, so that each member of the diving team can select what they think is needed. Each procedure will add or subtract life (MoLA) to the life timer.
   * 7.4 The selected life-saving procedures will take time to execute. When  “surfacing”, the team is replaced by NPCs or other players may take over. A patient bed is blocked for the amount of time the real procedure would take, including NPCs working on the patient.
   * 7.5 Each player can see his own performance gauge (speed/accuracy) and is also be able to see the overall team performance gauge.
   * 7.6 Grand challenge.

## Development Process

Case cards will be sorted into scoring systems and designed for titrated challenge for players. The augmented reality block emergency unit simulation will be detailed and technical specifications documentation will be completed for the design vendor. This includes a description of how simulated patients will flow through the system, how their life paths and outcomes will be recorded and how player actions will influence this flow. Translation and accessibility options will be introduced.

Card and Challenge Titration Specifications, each case card will be assigned a scoring value and integrated with rate of patient flow adjustment. Levels or other indicators of progress will be designed to provide analytics for players. 

Concept Art and Hedonic Design. The player interface will be integrated with analytics in the Leaderboard. Artwork will integrate with in-game actions describing patient flow dynamics, control of experience intensity and scoring systems. A splash launch screen, integration with LMS portals and player token management. 

###
