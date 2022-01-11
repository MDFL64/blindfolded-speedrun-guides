# Portal Blindfolded Route

## Practice Runs

Twitch deleted my old videos. I may or may not resume trying to route this in the future.

## Category

I intend to use glitches if they're viable, but out-of-bounds and save glitch are both probably not. Right now I'm shooting for the "No SLA" category.

Glitches used:

- Portal bumps

Future potential glitches:

- Prop climbing
- Glados turret damage

## Existing Runs and Strategies

[Katun24](https://www.youtube.com/watch?v=PMIFB9pmZYs&t=236s) completed the first (and only?) blindfolded Portal run in 4:34:35.

Reddit user [L4sgc](https://old.reddit.com/r/speedrun/comments/6m5ydu/i_am_routing_for_a_portal_1_blindfolded_run/) routed the first 13 chambers.

The Portal speedrunning community maintains a [very nice document](https://docs.google.com/document/d/1H7AHqiSTRzJE2xfqPCGBsUXZay1g9wdUfCbPXoz8S3c/edit#) with tutorials for different categories.

Youtuber UncraftedName has a [playlist](https://www.youtube.com/playlist?list=PLgZsR4Jh0IEm1ZPj3JGX_hkoZow9EdUET) of strats for the no-pass-through-portals category. A lot of the later chambers use save glitches that are too hard to line up, but there may be some useful stuff here. The [least portals segmented run](https://www.youtube.com/watch?v=BwCY_Bwx3-g) may be useful for the same reasons, but it uses a ton of crazy launches that would be impossible in an actual run.

Imanex completed a "no mouse movement" run which can be found [here](https://www.youtube.com/watch?v=UvtA_-BLUzE). A lot of these routes end up being more complex than just aiming a shot, but there are some things worth stealing, and a more competent runner willing to memorize more might find some success with these strats.

## autoexec.cfg

Hopefully everything here is okay. Katun24 requested `cl_mouselook` to be allowed, and while it was never explicitly approved, I'm going to assume it's fair game since it enables a similar config he used in his run. I assume `cl_pitchspeed` and `cl_yawspeed` fall under "sensitivity binds".

I have also removed a bunch of the Glados VO sounds. This is allowed by the Portal speedrun community but still feels like cheating for a blindfolded run. 

```jsx
demo_interplimit 999999

// disable the mouse, start with zero cam speed
cl_mouselook 0
cl_yawspeed 0
cl_pitchspeed 0
// varying camera speeds
bind 1 "cl_pitchspeed 10; cl_yawspeed 10;"
bind 2 "cl_pitchspeed 30; cl_yawspeed 30;"
bind 3 "cl_pitchspeed 5; cl_yawspeed 5;"
bind 4 "cl_pitchspeed 90; cl_yawspeed 90;"
// look straight up/down
bind q "cl_pitchspeed 100000;"
```

## Chambers

I don't use much fancy notation. This might be a bit long and verbose, but I'd rather make this easy for myself and anyone else to read or edit

- WASD for movement, to distinguish from moving the camera.
- B/Y for portals once the dual portal gun is obtained.
- QCE for "quick crouch entry", a method of quickly entering downward facing portals. Most of the time I don't bother but it can be useful for normalization and some specific spots.
- @ [number] is used to specify the sensitivity bind.

### 00 (Wakeup)

- WA through portal
- AS 10 steps to corner
- WD 9 steps, on 10th step W until button
- D, pickup cube, SD until steps stop (possible to grab the cube as it falls if you time your movement and listen for the cue)
- A until button
- Place cube
- D, DS for adjustments to elevator

### 01 (Cycle 0)

- A, WA out of elevator
- S 4 steps, then careful S until glass steps
- Right 3 beats @ 1
- S to drop
- First portal after speech, W in portal, grab cube, S out portal, **SAVE** -- look out, portal can eat our cube
- next portal, W throw cube, throw cube -- retry as needed
- S out of portal, wait for transition, then W in portal -- speech can make this confusing and easy to miss the sound
- W to elevator

### 02 (Cycle 1)

- Hold S while: Left from "Please ... intend" @ 1
- W until doors open
- WA until stop, then quickly S + WA to enter portal
- W until portal gun
- Portal Down
- 2 tap W
- D until elevator

### 03 (Two Quick Ones)

- A, AS out of elevator
- Portal Down
- Save
- Right 7 portals @ 2
- D into portal, then AS, A to elevator.

### 04 (Pit)

**OUTDATED**

*Save glitch is probably doable for 4+5 but would be very difficult to line up. Probably slower than doing both chambers normally.*

- D out of elevator until speech
- Portal Down
- Right 6 portals @ 2
- W into pit
- Grab cube, usually on the right side. Occasionally it will not be accessible and you'll need to turn a bit.
- Drop, portal, grab, W into portal
- Place cube on button
- Right 7 portals @ 2 — portal should hit
- D into portal, S, AS, A into elevator.

### 05 (Pit + 1)

**OUTDATED**

- D, DS out of elevator
- Portal Down
- Portal
- Back through portal -- careful, need to push the cube a bit, can check by tapping W
- Left 12 portals @ 2
- Grab cube
- W off platform
- A to button
- Place Cube
- WD into pit
- AS to corner
- D + Use to grab cube
- Drop, portal, grab, W into portal
- W off platform
- D to button
- Place Cube
- WD throught door
- Portal Down
- S to elevator

### 06 (Pellet)

F*all to exit platform is viable, but is inconsistent, dangerous, and saves only ~10 seconds.*

- W past billboard buzz
- WD into corner -- wait for:
- SA "aperture science"
- WA at "Must" until on platform
- W into elevator. **SETUP REQUIRED FOR NEXT CHAMBER!1z**

### 07 (Pellet + Platform)

**OUTDATED - Reverted to old strat.**

*I spent way too much time trying different strats for this chamber. Launching and strafing through a portal on the wall are both possible, but super inconsistent. Prop climbing using the radio seems like a pretty good fast option, but getting to the radio and rotating the camera are time-consuming. Probably the fastest viable option is to just climb the scaffold support. A more skilled runner could probably pull this off, but I struggle to do this when I can see. Any variant of the intended strat requires a difficult lineup.*

- S to speech. 5 left @ 1 while S.
- A/S/D to edge of portal-able on wall, under platform.
- W 8 steps until metal steps.
- Save, D into portal. Make sure you're on the platform.
- Save, 7 down @ 2. May need to move left or right and retry.
- BACKUP:
    - Move to upper-right corner of un-portal-able.
    - Down/Right 2 shots @ 1
- Wait for scaffold to reach far side, or for end of speech, SAVE.
- A + jump off scaffold. Retry as needed.
- AS to elevator.

### 08 (Pellet + Platform + Gunk)

*Might be possible to use fast strat of jumping on the block and strafing, but takes longer to setup and is more difficult to do blind.*

- WD → "Failure"
- AS back a few steps.
- QCE into portal down.
- Left 2 portals @ 2.
- Left 7-8 portals @ 2 to edge of portal-able.
- Left 3 portals @ 1. Listen for orb bounce to Left.
- Left 4-5 portals @ 1. Listen for orb catcher.
- Save and wait for platform. If your position is bad you might get pushed off by the catcher.
- W/WD into elevator.

### 09 (Impossible)

**OUTDATED**

*Glados is VERY annoying on this level. Fortunately I re-routed this so you need a minimal amount of rotation, and don't need to listen for portal hits.*

- AS out of elevator. Jump, portal down, look UP. Radio should be to your RIGHT. You should be facing the portal, so it shouldn't be portal-able.
- D/ WD / W to find cube.
- Jump, Portal, W to wall, place cube inside portal.
- SD through fizzler, then D onto button.
- Portal. W to wall, then grab cube.
- S back to button. Place cube.
- W back into cube, careful not to push it off the button.
- D / WD to elevator. The elevator makes a loud noise when you reach the bend in the hall.
- W into elevator.

### 10 (Fling Intro)

- S out of elevator.
- Jump into portal down.
- W through door until wall. S until portal down.
- Look up, W through portal.
- Look up, S through door to wall.
- Place portal as high as possible (7 down @ 1). **SAVE**
- W through portal, hold look down. Don't need to hold crouch BUT holding W/S after going through portal can screw this up. Retry as needed.
- W into elevator. **SETUP REQUIRED FOR NEXT CHAMBER!**

### 11 (Cycle 2)

- Before start of chamber:
    - Position aim down, then up 4 @ 2
    - Be aligned with the back of the elevator
- S out of elevator for 8 portals.
- Wait for portal to change.
- W, crouch jump into portal.
- W to portal gun.
- Press button and place B through door. (Down ~6 @ 2) **Make sure you don't place a portal inside the orb catcher.**
- Crouch 3 steps A.
- W + hold jump + spam Y
- B on opposite wall.
- Y down to setup for next chamber.
- WD into elevator.

### 12 (Fling Climb)

- 15 steps A
- Up Y from bottom @ 2 to highest portal-able. Can also go down ~3 portals @ 2.
- W into pit, then S to wall.
- Up 2 B, until portal-able. Must stop at the edge.
- W through portal, immediately shoot Y. Should fall back through our portal.
- Look up, then go down 4 Y @ 2.
- WD to button, then back off button. Backup: AW to corner, SD to button.
- S slowly, spamming Y until hit.
- S, look down, B on ground.
- Fix view (down 4 @ 2), A to cube, grab. Should hear it drop from the dispenser.
- S down to previous platform. SD to corner, AW to button. (Do not use Left corner, wall has weird geometry!)
- Place cube.
- D, W into pit, look down, B on ground.
- D to elevator

### 13 (Long Time)

- A to wall, then SD to corner.
- S to wall. Should pass over button.
- Portal up for 5 steps A.
- Portal down.
- Level camera with 6 portals @ 2.
- S, Crouch, jump, spam use until the cube is held.
- S, **SAVE**, cube throw with B + use. Retry until door opens.
- WA into door 5-6 steps. Should hear metal steps. W to far side of door.
- Left 10 Y @ 2. Right Y to edge of portal-able.
- AS onto cube/button. Grab cube.
- A to wall.
- Drop cube, B, grab cube.
- W through portal.
- Place cube on button. May be easier to crouch and check if cube hits.
- **SAVE**
- Left 9 Y @ 2.
- W to ground. B down. W to button. Make sure the door actually opens.
- Left 6 Y.
- Right @ 1 as far as possible until no-longer portal-able. **WARN:** Walls on both sides of the door are portal-able.
- Fall off platform. B down.
- Sanity check: shooting a portal here should knock camera off the wall.
- D into elevator.

### 14 (Easy Skip)

- A out of elevator to wall.
- S slowly back, place Y down at edge of portal-able.
- S back, place B up at edge of portal-able.
- W through portal, place B down.
- After passing through second portal, S back to platform.
- D/DS into elevator.

### 15 (Bunch of short chambers glued together)

**FLING 1**

- A out of elevator to sign.
- AS to corner.
- Down/Right 4 Y @ 2.
- B down.
- B down, Look up AFTER through first portal.
- Portals should fizzle. Orb should be to our RIGHT.
- S to wall.

**ORB**

- D to wall & up 3 portals @ 2 while walking. Wall should be portal-able until you reach the end.
- Right 3 Y @ 3, then slowly move right. Non-portal-able sound will change if you move too far.
- QCE B down, or enter normally and backup to wall.
- Left 6, then up 3 Y @ 2.
- Alternately place Y THEN B until the blue is placed. Y down.

**FLING 2**

- Look up, then left 6 B @ 2.
- A to wall. Should pass over metal.
- D, Y until portal-able down.
- Through portal, B down, D through fizzler.

**HALL OF DOOM**

- Portal forward (try hitting the panel, otherwise level your view and hit the wall at ground-level)
- Portal down so you're facing the angled walls the orb bounces off of.
- A into the hallway. Might take some trial and error.
- Y forward.
- Left 6 B @ 2.
- **SAVE, be careful with save states here.**
- D/crouch into portal, B, A back.
- D/crouch into portal, look up, 12 shots @ 2.
- 6 shots down @ 2. SAVE, then try B, D back.
- A through portal. Should hear platforms move.

**PLATFORM ROOM**

- QCE Y down so we're facing the tunnel.
- D to wall, A to edge of portal-able down, place Y. Careful not to fall through.
- A+jump over portal, A to portal-able UP.
- D into portal, B down, A onto platform.
