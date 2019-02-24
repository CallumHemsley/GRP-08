---
title: Meeting Diary
layout: post
---
## 2019.02.24
1.	Work Report
	1) Harrod: build a dialog system by Unity & upload to GitHub; background research – cYark (Website) & Lost Palace of which we can learn the idea of IMMERSIVE.
	2) Callum: simple character movement & auto saving by each 20s & quit 
	3) Yuming & Yuhao: UI construction; frame-by-frame animation; collect some graphic components which might be used.
	   * the art style of the game should be similar which means the buildings, the components and the GUI should be in a similar style.
	4) Jianglun & Yuyu: historical knowledge gathering
2.	Work Distribution
	1) Historical knowledge gathering and preparation – Jianglun & Yuyu DDL: 2.27 before regular meeting.
	2) Game sketch level & animation – Callum & Harrod
	3) One simple scene building up & graphic components gathering – Yuhao & Yuming

## 2019.02.20
1.	Feedback to interim report:
 	Team members should be focus on the detail, including:
	1)	the background survey of any existing systems that address similar problems; 
	2)	market research; 
	3)	technical research of platform choice, tools algorithms and data structure; 
	4)	initial implementation steps.
2.	Working plan:
	1) Arrange meeting time for group member.
	2) Finish the implementation of game framework.
	3) Everyone should work on 4 or 5 surveys and combine the result.
3.	Answer for question:
	1) UI component should be made by Unity.
	2) The suggestion of building texture will be given after finishing the game framework. 

## 2018.12.21
* Team has set up a github repo for the unity project, inlcuding a gitignore file so commits won't have lot's of conflicts.
* Over the next two weeks the team must do:
    * Initial coding implementation, on GitHub.
    * Start working on textures and structure of the levels.
* Also discussed what we would do over winter break, which is from 19th Jan until 17th Feb.
* 2 members of the team were not at the meeting, therefore we will have another meeting to plan how to divide the work for implementation.

## 2018.12.12
* Clarified issues within group report draft:
    * UI contradictions were changed.
    * Font sizes was clarified as 1-5.
    * Volume was clarified as 0-10.
    * Prototype contradictions changed.
    * Changed UML to more accurately match requirements.
* Content table is needed at the start, with sections and subsections.

## 2018.12.5
* Some errors are in the initial report:
	* prototype should be a separated section
	* chosen platform belongs to the background part
	* the order of the report should better be design --> prototype --> implementation
* platform: we decide only develop Android version.
* Both the diagram size and the text size should be larger than before.
* the intiicoding should be included, and the results should be taken as screenshots.
* future plan, Gannt chart, aim (purpose), overview and motivation (promote traditional culture and protect historical heritage)  should be added


## 2018.12.2

* decide to change the game mechanism again:
	* collections are the scrolls
	* they could see the photo of Tianyi pavilion in the game
	* if they give a wrong answer for the quiz, NPC will directly show the answer to them if they don't want to change their answer.
	* scrolls could only be collected by the player when they have found them. If they answer the wrong question without the scroll, they won't get the scroll in that room anymore.
	* answering the quiz right or wrong decides their final score of the game.


* visit mode has several changes
	* it can not unlock all the scrolls(collections) 
	* firstly, the user chooses which building to visit
	* secondly, introduction of the building，scrolls of the building, photos could be chosen. Those items are shown as labelled-lists.

* Tuesday night each one of us should finish our own part. Before Wednesday's meeting we should use latex to combine our work together

## 2018.11.28
*	Discussion about the order of chapters – leave it for now
*	Discussion about the report 
	* each one explains his own work like UML & UI; 
	* each one start to write his own part – DDL 12.2
*	pictures of the real scenes – leave it for now
*	prototype – Game UI : draw the draft ( NPC position & Door Position) One screen – one room
*	Simple Unity 2D Coding for character move – Yuyu DDL 12.2

## 2018.11.25
* Discussion about the construction of our game, based on Minghao’s opinion,Reconstruct the construction:
	* each building should have a sub-lobby
	* each room should have a NPC 
	* different NPC have different functions – lobby NPC gives building keys; sub-lobby NPCs give own rooms’ keys; room NPCs give quizzes.
	Based on this, draw the class diagram.
* Database discussion
	*	How to save coordinates? 
	*	How to interact with NPC? – check the range within the character and NPC automatically
	*	What kind of data should be saved? – anything will be invoked from database.
		* i.	Building ID - int
		* ii.	Room ID - int
		* iii.	Coordinates – double
		* iv.	NPC ID – int
 		* v.	Scroll ID – int
		* vi.	Quiz ID – int
		* vii.	Key ID – int 
		* viii.	Door ID – int
		* ix.	Etc’s ID – ID
		* x.	Building Name – String
		* xi.	Room Name – String
		* xii.	NPC Name – String
		* xiii.	Scroll Name – String
		* xiv.	State of objects – (Boolean)
		* xv.	Number of keys – int
		* xvi.	Number of Scrolls – int
		* xvii.	Number of the exact keys of which character owns – int
		* xviii.Number of the exact scrolls of which character owns – int
*	In case of segmentation fault - > build separate maps instead of one single map
*	UML & UI: re-modifying
*	An object called options need to be added, since it is aggregated with Quiz.
*	Quiz – based on the real history



## 2018.11.21
What we need do in next week:
   * Generate out database of App
      * Design the data structure: what will be included
   * Finish the class diagram
   * Make UML diagram more detail
   * Do some background information research
   * Do some modification base on the feedback
* Database structure:
   * Save the game state: character coordinate, prefer setting and so on, may use table or array to store it
   * Fifure out the key variable in the game and store it
   * The content of quiz and scrolls, if the question is same, put in the code but database
* Background information:
   * The information about TianYi pavilion which put into scrolls
   * The quiz asks some knowledge about the information in scrolls
* Task reallocated:
   * Background information research & time plan & updated and expanded description of problems: Yuyu Hu
   * Requirement specification & Meeting Records: Minghao Wang : Minghao Wang
   * Results of any initial implementation steps/prototyping: Jianglun Huang
   * Record of key implementation decisions, such as programming languages etc.: Yuhao Chen
   * Discussions of problems encountered so far, both technical and management issues: Callum
   * UI and initial design of proposed system: Yuming Zheng
* Maybe there are three room per building, nine in total
* Report need be finished one week before the DDL
* Have a meeting at Sunday


## 2018.11.20
* Activity Diagram:
    * Delete score system
    * Add turn on/off voice action
    * Add auto save
    * Add share action in collection page
* Use case diagram:
    * Add manual save, put in menu
    * Add intend and extend keyword
* Share action:
    * Share the number of collection or the content of collection to WeChat/Weibo
    * In collection page: after sharing, go back to collection page
    * When play game: can be found in menu
* Visit Button(in menu):
    * VR picture 
    * VR video   
* VR picture & VR video
    * Transfer normal video/picture to VR vedio/picture
    * Or Create by ourselves
    * Unlocked if:
        * User choose to visit
        * User choose to play but have collected all scrolls

##  2018.11.16
* Activity Diagram:
   * Actor: Visitors
   * Visitors Activity: 
      * Settings (language, voice guidance, font size)
      * Save game record
      * Play or Visit
      * Choose chapter of the game (buildings)
      * Guidance
* Sequence Diagram:
   * Setting (language, voice guidance, font size)
   * Choose Play & Visit
   * Procedure of playing:
      * Enter the lobby, NPC will give them corresponding key->
      * Get into the chapter(building) ->
      * Find NPC in the first room, get the quiz ->
      * Answer the quiz, or go to find the scroll ->
      * …………………………………………………..
      * Below are for decision of finding the scroll
      * (collect the scroll ->) 
      * (read to find the answer ->) 
      * (answer the quiz ->)
      * Above are for decision of finding the scroll
      * ……………………………………………………
      * pass => (get the scroll) ->
      * fail => (educate: by highlight the position, don’t get the scroll) ->
      * NPC gives the next room’s key 
      * next room: the same pattern as the first room------> 
      * final room: the same pattern, but will not give next room’s key -> 
      * if it is (TianYi pavilion), gives the final score, if they are willing to share the final score, unlock all collections they don’t have. Otherwise, remain the same. Go back to the menu.
      * If the building is not Tianyi pavilion, the player will be sent back to the lobby. They could choose to continue or exit the game.
* Overall arrangement of the map
   * A Lobby ‘O’ and several rooms ‘A’, ‘B’, ‘C’, like a tree
   * And a series of room ‘a1’, ‘a2’, ‘b1’, ‘b2’, ‘c1’, ‘c2’
   * The lobby can only access to ‘A’, ‘B’, ‘C’, ‘A’, ‘B’, ‘C’ can’t access among each other
   * ‘A’ can access to ‘a1’, ‘a1’ can access to ‘a2’, like an array. Same as ‘B’ and ‘C’
   * NPCs are in each room
   * It’s able to quit and automatically save. That will move players to the main room O
* Language: Unity, Csharp
* Tasks:
   * Use case diagram: Minghao Wang
   * Activity diagram: Yuming Zheng
   * State machine diagram: Callum
   * Sequence diagram: Minghao Wang
   * Prototype: Yuhao Chen, Jianglun Huang
   * Background research: Yuyu Hu
   * DDL: Tuesday 11.20 6pm
   * Have a meeting at Tuesday 11.20 night at Yuyu’s dorm


##  2018.11.14
* This week we focus more on our course work as there are 2 DDLs during this week.
* Our question according to the mid term report:
    * We have no idea how much we are supposed to do in the report, and how much we should do in this term.
    * There is no concrete format of the report
* ----write as far as we did in the report
* How current problem in the whole project:
    * No clear timeline now
    * No short term plan now (what to do these days among requirement specification, UML, and prototype)
    * No fixed unofficial meeting time
    * No communication between us
* Solution:
    * Discuss the above problem in the weekend

##  2018.11.07
* Requirement part: 
    * For the key feature of the building: add more details about the building, for example: the construction time of building, which include the different architectural style of different periods. 
* Specification part:
    * It is fine to use multi-media to improve user's immersive experience, for instance: the traditional Chinese music, bilingual text guidance, and bilingual audio guidance. 
* Software & programming part:
    * Group member should all agree with the software that going to use and define the role by facility.
    * It is suitable to create the game in 2D way regarding the Hardware & Software situation. 
* Interim report:
    * Words limit: the words of interim report can be more than 5000 words, of which our marks will have not deduction.
    * Group member should create the UML, prototype and the UI.
    * Complete the requirement and specification, and the format of it is in the previous year lecture slides.

##  2018.10.30

  This week, our supervisor is in UK so meeting over WeChat voice call.

  Introduction on our current state:
* We went to Tianyi Pavillion to take photos of buildings.
* There was a problem with the 3D software "reality capture":
    * To buy is very expensive, around 40,000 RMB.
    * We are trying the free version currently.
    * We are also unsure on how long this license for 40,000 RMB lasts e.g 3 months, the whole year etc.


  We are currently making the requirements specification now.



  Following that this week we will create some UML.


  Due to software being so expensive, we are thinking about pursuing different options in order to make the application immersive.
  One such example is using 2D design instead, which allows for us to create more interactions for the user.


  Website deadline is for the 31st October. (We have already set this up)


  marking of the website is on 1st November.



##  2018.10.23
  1. We've decided three building as our modelling targets.  The first one is TianYi Pavilion. The other two are next to it. 
  2. Positions of each team member are confirmed. They might be changed in the future.
    - Script - Minghao & Yuyu 
    - Modeling - Yuyu 
    - Website - Minghao
    - UI - Yuming
    - Testing - Callum
  3. We planned to take photos of these three buildings and their surroundings this week.
    
    
##  2018.10.17
  The second time we met with our supervisor. She told us to decide how many buildings and which buildings did we prefer. My team decided
to go Tianyi Park and then made decisions.
