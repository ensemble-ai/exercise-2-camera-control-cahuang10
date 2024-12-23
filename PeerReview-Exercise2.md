# Peer-Review for Programming Exercise 2 #

## Description ##

For this assignment, you will be giving feedback on the completeness of assignment two: Obscura. To do so, we will give you a rubric to provide feedback. Please give positive criticism and suggestions on how to fix segments of code.

You only need to review code modified or created by the student you are reviewing. You do not have to check the code and project files that the instructor gave out.

Abusive or hateful language or comments will not be tolerated and will result in a grade penalty or be considered a breach of the UC Davis Code of Academic Conduct.

If there are any questions at any point, please email the TA.   

## Due Date and Submission Information
See the official course schedule for due date.

A successful submission should consist of a copy of this markdown document template that is modified with your peer review. This review document should be placed into the base folder of the repo you are reviewing in the master branch. The file name should be the same as in the template: `CodeReview-Exercise2.md`. You must also include your name and email address in the `Peer-reviewer Information` section below.

If you are in a rare situation where two peer-reviewers are on a single repository, append your UC Davis user name before the extension of your review file. An example: `CodeReview-Exercise2-username.md`. Both reviewers should submit their reviews in the master branch.  

# Solution Assessment #

## Peer-reviewer Information

* *name:* Stephanie Hsia
* *email:* sehsia@ucdavis.edu

### Description ###

For assessing the solution, you will be choosing ONE choice from: unsatisfactory, satisfactory, good, great, or perfect.

The break down of each of these labels for the solution assessment.

#### Perfect #### 
    Can't find any flaws with the prompt. Perfectly satisfied all stage objectives.

#### Great ####
    Minor flaws in one or two objectives. 

#### Good #####
    Major flaw and some minor flaws.

#### Satisfactory ####
    Couple of major flaws. Heading towards solution, however did not fully realize solution.

#### Unsatisfactory ####
    Partial work, not converging to a solution. Pervasive Major flaws. Objective largely unmet.


___

## Solution Assessment ##

### Stage 1 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justification ##### 
Position lock works fine! Camera centered on vessel.

___
### Stage 2 ###

- [ ] Perfect
- [x] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justification ##### 
The box auto scrolls on z-x plane but when controlling the vessel sometimes it drifts when not intended to.
The vessel moves in the direction of the frame when touching the left and right borders relative to the direction it's scrolling.

___
### Stage 3 ###

- [ ] Perfect
- [ ] Great
- [x] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justification ##### 
The camera catches up to the player when the player is not moving but when testing I don't think the leash is working correctly. The vessel just keeps moving further and further away from the center of the camera if it doesn't stop.

___
### Stage 4 ###

- [ ] Perfect
- [ ] Great
- [x] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justification ##### 
The camera does move (in the direcrtion of movement) faster then the vessel and leads but the camera just keeps going if vessel keeps moving (no leash). Delay works and camera catches up after delay.

___
### Stage 5 ###

- [x] Perfect
- [ ] Great
- [ ] Good
- [ ] Satisfactory
- [ ] Unsatisfactory

___
#### Justification ##### 
Pushbox and speedup zone works as intended. Accelerates within speedup zone, pushes box at edge, stops when within the center box. Perfect job!
___
# Code Style #


### Description ###
Check the scripts to see if the student code adheres to the GDScript style guide.

If sections do not adhere to the style guide, please peramlink the line of code from Github and justify why the line of code has not followed the style guide.

It should look something like this:

* [description of infraction](https://github.com/dr-jam/ECS189L) - this is the justification.

Please refer to the first code review template on how to do a permalink.


#### Style Guide Infractions ####
[Some lines](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/speed_push_zone.gd#L51) are over 100 characters

[Stage 3 camera](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/stage_three.gd#L1) could be renamed for its use to be clearer.
Another small point on naming is all the cameras could be renamed with camera added as well. As the cameras given to us was named "PushBoxCamera".

#### Style Guide Exemplars ####
Great job with the [order and the declaration of variables](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/speed_push_zone.gd#L4) and naming conventions. It follows the style guide closely.

Amazing job with following the style guide!
___
#### Put style guide infractures ####

___

# Best Practices #

### Description ###

If the student has followed best practices then feel free to point at these code segments as examplars. 

If the student has breached the best practices and has done something that should be noted, please add the infraction.


This should be similar to the Code Style justification.

#### Best Practices Infractions ####
The script files for the cameras where placed in random folders and not organized together in the script/camera_controllers folder.

[Some variables](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/speed_push_zone.gd#L38) were declared but never used.

More comments would be great! For example, for the [draw_logic function](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scripts/camera_controllers/postion_lock.gd#L24) in each camera, you can mention which border/line it is.

Maybe use helper functions to [check boundaries](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/speed_push_zone.gd#L50) in Speedup Push Zone camera for better readability.

And I noticed only 1 commit, having the habit of committing often is great! (Something I also need to work on...)

#### Best Practices Exemplars ####
Consistently [declared variables](https://github.com/ensemble-ai/exercise-2-camera-control-cahuang10/blob/2a9d8cd031bc7124a4e4ca5e8aec831bc6a97306/Obscura/scenes/auto_scroll.gd#L37) near where they are used, and used local variables when they aren't needed globally.

No major problem overall! Good job!
