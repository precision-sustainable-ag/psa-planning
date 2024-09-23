# psa-roadmap

**Date Created:** 06/01/2024

**Date Last Modified:** 08/30/2024

The psa-planning repo is the place where big picture Precision Sustainable Ag (PSA) planning milestones and epics are stored. These are then visualized in the PSA Planning GitHub Project linked here https://github.com/orgs/precision-sustainable-ag/projects/5.

## Breakdown of item subtypes

There are 3 main types of planning items, 2 of which are stored in this repo. 
1. Tasks: The smallest planning unit. These items do not live in this repo. Instead, they are spread out amongst lots of repositories in the PSA organization. A task is an item taht is scope to be assigned and completed by a single person. It has all of the technical details needed to complete it.
2. Epics: An epic is a collection of tasks. It is a larger unit of planning that links to multiple tasks in external repos. It does not go into the same level of technical detail, and is typically filled out by a project manager or a tehc lead. All epics live in this repository.
3. Milestones: These are the largest planning unit. Each milestone is a collection of epics. These are items that may take months or years to complete. All milestones live in this repository.

## Label automation using Github Actions
Every time an issue is created or an issues labels change, a Github Action runs that adds the issue into the PSA-Planning project linked above. It also parses the labels that start with `project: ` or `team: ` and assigns whatever comes after to either the Team or Project column in the Gihub Project.

For example: if a new issue is created with the labels `team: DST` and `project: DST-selector` then the action will perform 3 tasks.
1. It adds the issue to the PSA-Planning Github Project
2. It assigns the Team field to `DST`
3. It assigns the project field to `DST-selector`

This avoids several manual clicks that would otherwise be needed for every issue.

## Limitations
1. An epic can only be assigned a sing team because GitHub Projects do not support multi select fields yet. This is currently one of the most requested features on GitHub community, so hopefully it will be added soon. Vire here for more details https://github.com/orgs/community/discussions/6580.

## Example GitHub roadmap built from these items

![2024-08-30_10-18](https://github.com/user-attachments/assets/667342e5-6a15-474d-a820-5d352f35933e)

## Example GitHub Kanban board created from these items

![2024-08-30_10-22](https://github.com/user-attachments/assets/44ba32b9-e7ab-4174-bf85-f329837aece9)

## Advantages of this system

1. It allows for a roadmap to be created for PSA as a whole and viewed in one place instead of fractured project management tools across multiple teams.
2. It can directly link out to tasks in external repos, making it very easy to go from the top level all the way done to a specific task's conversation and documentation.
3. You can see who the owner of an epic is quickly and easily on the roadmap.

## Glossary of useful terms
1. DST: Decision Support Tool
2. PSA: Presision Sustainable Ag
3. SCCC: Southern Cover Crops Council
4. NECCC: Northeast Cover Crops Council
5. MCCC: Midwest Cover Crops Council
6. WCCC: Western Cover Crops Council
7. CRAFT: Citrus Research and Field Trials
8. GROW: Getting Rid of Weeds
9. PM3D: PlantMap3D
10. BBot: BenchBot
