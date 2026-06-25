---
name: session-scheduler
description: When the user wants to build or improve a camp's daily or weekly schedule, or design a themed program week. Use for a camp schedule, a daily or weekly timetable, balancing activities, rest and free time, transitions between activities, a theme week or culminating event, or fitting the day to different age groups. It draws on camp-overview for the camp year and camp-profile for the camp's ages, facilities, and staff. Schedules must fit the camp's own supervision ratios and jurisdiction.
summary: Daily and weekly schedules and themed program weeks.
category: programs
icon: tent
examples:
  - "Build a daily schedule for a day camp with three age groups."
  - "Plan a five-day pirate theme week with a big closing event."
  - "Balance free time and structured activities for a cabin of teens."
order: 8
status: published
version: 1.0.0
---

# session-scheduler

Build a camp's daily and weekly schedules and themed program weeks so they fit the group, the facilities, and the staff. This carries camp program-design best practice with the camp's own constraints layered on top.

It is written for you, the agent. Use camp-profile for the camp's ages, facilities, and staff, and camp-overview for the camp year. A seasoned director often knows their camp better than any general source, so the value here is a solid draft fit to their ages, site, and traditions, plus a check on the things that quietly break a schedule (ratios, rest, transitions), not generic advice. The block lengths and timings below are conventions, not rules, and the supervision ratios must follow the camp's own jurisdiction and accreditor.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp type, ages, facilities, session structure, and traditions.
- Use camp-overview for where this sits in the camp year.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- The age bands and the group or cabin sizes, and whether any campers have support needs.
- Day or overnight, the session length, and the daily start and end times.
- The facilities and activity areas, and which ones different groups share (the bottlenecks).
- Staff headcount and specialists (lifeguards, climbing, riding), to check the ratio math.
- Fixed points: meal times, and any swim, rest, or assembly already set.
- The traditions and non-negotiables to keep, and, the most useful question for an experienced director, what has not worked before: the chaos points, the blocks campers disengage from, the transitions that fall apart.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to a solid daily schedule, and offer to go deeper.

- **Quick wins (low effort):** a strong daily schedule for the main age group.
- **Solid setup (medium effort):** the full daily and weekly schedule across the age bands, with transitions, rest, and meals built in.
- **Full build (high effort):** the season's themed-week arc plus the schedule and the staffing and ratio math.

## Build the schedule

### 1. Design the day around energy (all tiers)

Sequence matters as much as content. A camp day runs in a rough arc: higher energy through late morning, a structured midday, a deliberate dip after lunch, and a wind-down before pickup or the evening. Match activities to that arc. The post-lunch window (about 1 to 2pm) is the low point, so put calm, creative, or choice-based blocks there (art, free swim, journaling), and save the hardest physical activity for the mid-afternoon rebound.

### 2. Fit blocks and transitions to age (all tiers)

A block can only run as long as the group's attention holds. As a convention, younger campers (5 to 8) hold a block for about 30 to 45 minutes, 9 to 11 for 45 to 60, and 12 and up for 60 to 90 on project or skill work. Plan a real 10 to 15 minute transition between blocks. Transitions are designed time, because the gaps between activities are where days fall apart and where behavior incidents cluster.

### 3. Protect rest, downtime, and free play (all tiers)

A structured quiet or rest period (the classic post-lunch rest hour, 20 to 30 minutes) is a program element, not dead time, and it pays off in afternoon behavior. Unstructured free play is developmentally necessary, not indulgent (the American Academy of Pediatrics is clear on this), and fatigue across a session is a real safety and behavior issue. Over-programming every minute is a known failure mode, so resist filling the gaps.

### 4. Balance and anchor the day (Solid setup)

Alternate high and low energy, and structured blocks with real choice, so campers are not held at one intensity all day. Choice and camper voice build belonging and a sense of mattering. Use meals as the day's fixed points, with the activity blocks built around them, and as community moments (songs, announcements) that are part of the program.

### 5. Program for the age bands (Solid setup)

Camps group by developmental stage for a reason:
- **5 to 7:** short attention, imaginative play, unsettled by change. Short structured blocks, frequent gentle transitions, a predictable routine, close supervision.
- **7 to 10:** longer attention, peer socializing, skill mastery. Cooperative group games, clear rules, achievable challenges.
- **10 to 12:** peer acceptance and short-term goals. Team challenges and personal-achievement chances.
- **12 to 15:** independence and strong emotions, drawn to competing with outside groups. Skill specialization, group projects, respect for their emerging identity.
- **15 to 17:** want responsibility and to be treated as young adults. Leadership and counselor-in-training roles, real responsibility.

### 6. Check the staffing and ratio math (all tiers)

Every concurrent block needs enough qualified staff to hold the supervision ratio for that age, so when a schedule splits groups or runs parallel activities, do the math. Ratios are set by the camp's jurisdiction and accreditor, not by this skill (for ACA guidance and the figures, and where to confirm yours, see `references/schedule-design.md`). Specialist activities (waterfront, climbing, riding) need their qualified staff slotted in, and staff breaks and time off have to be woven into the grid, not bolted on.

### 7. Arc the themed week and the season (Full build)

A theme should be broad enough to feed four or five different activity types (a physical challenge, a creative project, a team game, a group ritual, a recurring daily anchor) and build toward a culminating event. Across the season, open strong with a high-energy week, vary active and creative themes, and place the quieter themes mid-summer when camper and staff energy dips. Pick themes from the campers' age outward, not the director's taste, and brief counselors about a week ahead so supplies arrive in time.

### 8. Design for development and inclusion (Solid setup)

A strong schedule meets the recognized features of a positive developmental setting: physical and psychological safety, a clear but not rigid structure, supportive relationships, chances to belong and to matter, skill-building, and positive norms (Eccles and Gootman). Build in inclusion: predictable routines, a quiet or sensory-regulation space, and activities with more than one way to take part, so a camper can choose a lower-stimulation version rather than only being in or out. Make sure competition structures like a color war do not leave the same campers or cabins chronically on the losing side.

## Deliver the schedule

- Give a clear daily and weekly grid (or block list) fit to the camp's ages, facilities, and staff, with rest, transitions, and meals built in.
- Show the ratio math for any block that splits or runs parallel groups, and flag where the plan depends on a facility or a specialist being free.
- For a themed week, give the arc and the culminating event.
- Say plainly that it is a starting point to adjust once they see how each group actually moves, and hand any parent-facing schedule message to camp-emails.

## What this skill will not do

- State a supervision ratio as a universal legal minimum. Ratios follow the camp's jurisdiction and accreditor; confirm them.
- Over-program the day, or cut rest and free play to fill gaps.
- Schedule beyond an age band's attention span or physical capacity.
- Slot a high-risk activity (waterfront, climbing, riding) without the qualified staff and ratios it requires.
- Override the camp's own traditions and constraints.

## Grounded in

Camp program-design and youth-development guidance. Block lengths and timings here are common conventions, not rules, and supervision ratios are set by the camp's jurisdiction and accreditor, not by this skill.

- American Camp Association, program standards and developmental traits: https://www.acacamps.org/accreditation/accreditation-overview
- Eccles and Gootman (2002), Community Programs to Promote Youth Development (the eight features of positive developmental settings): https://www.nationalacademies.org/read/10022/chapter/6
- American Academy of Pediatrics on the importance of play: https://publications.aap.org/pediatrics/article/119/1/182/70699
- Ontario Regulation 503/17, Recreational Camps: https://www.ontario.ca/laws/regulation/170503
