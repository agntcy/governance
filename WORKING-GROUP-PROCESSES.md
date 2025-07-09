This document describes the processes we use to manage the AGNTCY working
groups. This includes how they are formed, how leads are established, how they
are run, etc.

- [Why working groups?](#why-working-groups)
- [Proposing a new working group](#proposing-a-new-working-group)
- [Setting up a working group](#setting-up-a-working-group)
  - [Dissolving a working group](#dissolving-a-working-group)
- [Leads](#leads)
- [Running a working group](#running-a-working-group)
  - [Be open](#be-open)
  - [Making decisions](#making-decisions)
  - [Subgroups](#subgroups)
  - [Escalations](#escalations)

## Why working groups?

AGNTCY working groups are organizations responsible for the design and
implementation of large architectural aspects of the overall AGNTCY project.
Working groups operate with a fair amount of autonomy within the broader scope
of the project. They tend to be long-lived, representing major initiatives over
AGNTCY’s lifetime.

Some working groups focus on specific technologies. Other working groups are
cross-cutting in nature.

The steering committee is responsible for the AGNTCY project as a
whole. It sets the overall direction of the project AND, until such time where a
separate Technical Oversight Committee is formed, the steering committee helps make crosscutting
architectural decisions, helps establish and dissolve working groups, and helps
ensure all working groups are generally rowing in the same direction

Although working groups are relatively lightweight structures, we want to keep
the number of working groups low in order to keep things manageable.

## Proposing a new working group

If you've identified a substantial architectural area which would benefit from long-lived,
concerted and focused design, then you should consider creating a new working
group. To do so, you need to:

- **Create a charter**. This should be a few paragraphs explaining:

  - The mission of the working group

  - The goals of the working group (problems being solved)

  - The scope of the working group (topics, subsystems, code repos, areas of
    responsibility). Also it's very helpful to include items which are out of scope. The Steering Committee will be
    looking at this to make sure that there are appropriate touch-points and
    contracts between WGs when considering larger problems.

- **Nominate an initial set of leads**. The leads set the agenda for the working
  group and serve as final arbiters on any technical decision. See
  [below](#leads) for information on the responsibilities of leads and
  requirements for nominating them.

- **Prepare a Roadmap**. Create a preliminary roadmap (ideally, ~3 months worth) for what the
  working group would focus on.

- **Create a PR**. Create a PR for this repo with a new sub-directory under `working-groups` and add a 
  `CHARTER.md` file with your charter, nominated leads, and roadmap. The
  steering committee will evaluate the request and decide whether the
  working group should be formed, whether it should be merely a subgroup of an
  existing working group, or whether it should be subsumed by an existing
  working group. The PR should include the initial set of leads in a new section
  in [WORKING-GROUPS.md](working-groups/WORKING-GROUPS.md).
  
  - [example PR](https://github.com/agntcy/governance/pull/11)

## Setting up a working group

Once approval has been granted by the technical oversight committee to form a
working group, the working group leads need to take a few steps to establish the
working group._

- **Create a Google Drive Folder**. Create a folder to hold your working group
  documents within this parent
  [folder](https://drive.google.com/drive/folders/1l5v-aEArWGUL2_f79bx3ysizsRH2Z8PM?usp=sharing).
  Call your folder "GROUP_NAME".

- **Create a Meeting Notes Document**. Create a blank document in the above
  folder and call it "GROUP_NAME Group Meeting Notes".

- **Create a Roadmap**. Create a new [Roadmap Project Board](TBD) **TODO**.

- **Schedule a Recurring Meeting**. Create a recurring meeting (weekly or
  bi-weekly, 30 or 60 minutes) on the
  [shared calendar](https://calendar.google.com/calendar/embed?src=admin%40ops.agntcy.org&ctz=America%2FNew_York)
  and call the meeting "\$GROUP_NAME WG". Attach the meeting notes document to
  the calendar event. Generally schedule these meetings between 9:00AM to 2:59PM
  Pacific Time. Invite `<TBD>` Google group to the
  meeting, as well as necessary individual participants.

- **Register the Working Group**. Go to
  [WORKING-GROUPS.md](working-groups/WORKING-GROUPS.md) and add your working
  group name, the names of the leads, the working group charter, and a link to
  the meeting you created.

- **Announce your Working Group**. Send a message to [#agntcy-general on slack](https://agntcy.slack.com/archives/C0893S6D284)
  announcing your new working group. Include your charter in the message and provide
  links to the meeting invitation.

Congratulations, you now have a fully formed working group!

### Dissolving a working group

Some working groups are ephemeral or naturally reach the end of their useful
life. Working group leads can petition to dissolve their working groups by
emailing admin@agntcy.org.
The steering committee takes ownership of any artifacts created or
owned by the dissolved working group. The steering committee also
reserves the right to dissolve or recharter working groups over time as
necessary, though they will strive to first discuss this in committee meetings
and open community discussion.

## Leads

Each working group should have at least 2 leads, ideally 3, though young working
groups may have only 1 lead initially. Working groups should strive to include
representatives from multiple organizations as both leads and members. Working
group leads must be Members of the AGNTCY project (that is, have made multiple
contributions to the project in the form of code, design, or documentation).

Please see the [Roles](OPERATING_MODEL.md#3-roles-and-governance) defined in the 
governance operating model for a description of a lead’s role and requirements.

## Running a working group

Leads are responsible for running a working group. Running the group involves a
few activities:

- **Meetings**. Prepare the agenda and run the regular working group meetings.
  Ensure the meetings are recorded, and properly archived.

- **Notes**. Ensure that meeting notes are kept up to date. Provide a link to
  the recorded meeting in the notes. The lead may delegate note-taking duties.

- **Decision Log**. Ensure that significant design decisions are captured in
  GitHub issues, Google Docs, or markdown files in the repo.

- **Roadmap**. Establish **and maintain** a roadmap for the working group
  outlining the areas of focus for the working group, ideally, over the next 3 months.

- **Report**. Report current status to main community meetings or maintainers' meetings.

### Be open

The community design process is done in the open. Working groups should
communicate primarily through the public working group meetings, through design
documents in the working group’s folder, through GitHub issues, and GitHub PRs.
Avoid private emails and/or meeting when possible.

### Making decisions

In general, working groups operate in a highly cooperative environment. Working
groups discuss designs in the open and take input from the community at large
when making technical choices. The working group leads are ultimately
responsible for setting the direction of the working group and making the tough
technical choices affecting the working group.

### Subgroups

Subgroups are ad hoc subteams within a working group with a special focus on a
set of problems or technologies. We don’t formalize processes for subgroups,
each working group can decide when subgroups are needed and how they operate.

### Escalations

Working groups can get blocked on specific technical disagreements. Leads are
expected to generally resolve such issues and allow work to progress.

Sometimes, different working groups can have conflicting goals or requirements.
Leads from all affected working groups generally work together and come to an
agreeable conclusion.

In all cases, remaining blocking issues can be raised to the 
[steering committee](TBD) to help resolve
the situation. To trigger an escalation, create an issue in the **TODO**
steering committee's agenda (or email admin@agntcy.org) and be prepared to attend a meeting to provide
an explanation of the underlying problem as well as cogent arguments for both
sides.
