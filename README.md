# Harnessing Rust for Real-World Problems hackathon

## Introduction

This is a [hackathon](https://www.brightidea.com/guide/hackathon/what-is-a-hackathon/) for members of Calgary Rust, the user group for the Rust programming language in Calgary, Alberta, Canada.

## Purpose of the hackathon

The purpose of this hackathon is to help businesses (first and foremost, in Calgary!) solve their technical problems and demonstrate what [Rust](https://www.youtube.com/watch?v=5C_HPTJg5ek) is capable of.

## Duration of the hackathon

The hackathon will last for at least two days ([January 27](https://www.meetup.com/calgary-rust/events/298452155/) and [January 28](https://www.meetup.com/calgary-rust/events/298452254/)) but the participants can choose to continue working on the projects after the hackathon. This can be done, for example, at events organized by [Software Developers of Calgary](https://www.meetup.com/software-developers-of-calgary/) who host hackathons every month.

We have little in-person time for the hackathon but you can continue working on the projects remotely. Further, we will discuss how we are going to facilitate the remote communication between the team members.

## For newcomers to Rust

You're encouraged to start solving problems without hesitation. However, if you don't feel comforable jumping into the hackathon's projects right away, you can start by learning the fundamentals of Rust first. See [this](https://discord.com/channels/1090234243566817352/1164384007962755112/1164388726701555854) message in the [Discord server of Calgary Rust].

**Q:** Do we need to appoint any volunteers to help the newbies?

## Technicalities

Hackathon participants are encouraged to use [`git`](https://git-scm.com/) to collaborate on their projects. The projects can be hosted on GitHub, GitLab, Bitbucket, or any other platform that supports `git`.

Though this is a Rust hackathon, the participants are free to use any programming language they want. For example, this can make a lot of sense for frontend development or machine learning. However, you're encouraged to use Rust. By the way, you can also use native Rust modules in Python, JavaScript, and nearly any other programming language.

You are expected to self-organize to solve the problems. And you're encouraged to keep working on the projects after the in-person phase of the first day of the hackathon is over. To faciliate the communication between the team members, you're encouraged to communicate in the respective `#<project-name>` event channel in the Discord server of [Calgary Rust]. If you feel really motivated to complete the project and the project is big, you can also use tools like [Trello](https://trello.com/) or [ClickUp](https://app.clickup.com/) to organize the work.

## Problems

**Disclaimer:** the problems can be highly unstructured and require communication with the people who submitted them to clarify details.

### [Petrinex reports](petrinex-reports.md)

#### Team A

* Members:
  * TBD
* Repository: TBD
* Discord channel: [Calgary Rust] [`#petrinex`](https://discord.com/channels/1090234243566817352/1194995761142841394).

### [Website for Omnipedia](omnipedia.md)

#### Team B

* Members:
  * Michael McCulloch
  * ...
* Repositories:
  * <https://github.com/Omnipedia/RC-Hackathon-Website>
  * <https://github.com/Omnipedia/RC-Hackathon-ChatUI>
* Discord channel: [Calgary Rust] [`#omnipedia`](https://discord.com/channels/1090234243566817352/1194994891491659786).

### [Booking rooms for events](calgary-rust.md)

#### Team C

* Members:
  * Dmitrii Demenev
  * ...
* Repository: TBD.
* Discord channel: [Calgary Rust] [`#booking-rooms`](https://discord.com/channels/1090234243566817352/1194995158467485718).

### [Tailcall](tailcall.md)

#### Team D

* Members:
  * TBD
* Repository: <https://github.com/tailcallhq/tailcall>.
* Discord channel: [Tailcall](https://discord.com/invite/Q2ZExpFCnA) [`#contributors`](https://discord.com/channels/1044859667798568962/1156188728474214472).

### [Autodiff engine](autodiff-engine.md)

#### Team E

* Members:
  * TBD
* Repository: <https://github.com/GroupLabs/autodiff>
* Discord channel: [Calgary Rust] [`#autodiff-engine`](https://discord.com/channels/1090234243566817352/1196591774664228884).

### [Intel HDA UEFI Driver](intel-hd-audio-driver.md)

##### Team F

* Members:
  * Tait Hoyem
  * ...
* Repository: [TTWNO/hdaudio-uefi](https://github.com/TTWNO/hdaudio-uefi)
* Discord channel [Calgary Rust] [`#hda-uefi`](https://discord.com/channels/1090234243566817352/1195208855764865159).

### Other problems

[Algora.io](https://console.algora.io/) is a website for **paid** open-source contributions. It has a lot of problems that you can try to solve with Rust and for which you can claim bounties.

Notably, we have a privilege to have requests from companies like [Tailcall](https://github.com/tailcallhq/tailcall) and [Synnada](https://www.synnada.ai/) (who want contributions to <https://github.com/apache/arrow-datafusion>).

## Problem submissions

If you have a problem that you'd like to submit for the hackathon, please do so by creating a pull request to this repository. The pull request should add a Markdown file with the problem description. If you need assisstance with the submission of your problem, please contact `dmitrii_demenev` on Discord or e-mail `demenev.dmitriy1@gmail.com`.

[Calgary Rust]: https://discord.gg/N2vzPeADzn
[Discord server of Calgary Rust]: https://discord.gg/N2vzPeADzn

## Other questions

<details>
  <summary>Will the solutions to the problems be judged?</summary>
  
  Short answer, no. However, the teams will be encouraged to present their results.

  Judging would introduce even more complexity to the event planning. If we have other, more focused hackathons, it will be easier to invite/select a qualified judge or judges because the expertise would be narrower.

</details>

<details>
  <summary>What constitutes a finished project?</summary>
  
  It depends on such factors as...

  * **How (un-)structured is the problem statement?** If the problem statement is very concrete and the nature of the problem nearly perfectly fits the span of the hackathon, the project can be considered finished if it addresses all the requirements of the problem statement.
  * **Does the startup/business/third-party want to continue the project from there?** If the startup/business/third-party wants to continue the project from there, the project may end up becoming an actual product or an in-house project (e.g. a tool/[library](https://en.wikipedia.org/wiki/Library_(computing))). Then, the scope of the project may be extended and it will last as long as it brings the value and is maintained.
  * **Will the team of developers work on the project afterwards?**
    * If the team cannot continue working on the project after the hackathon ends and the soltuion doesn't meet the criteria in the problem statement, the project can be considered unfinished/dead/terminated. Though undesirable, such scenario still can be valuable.
    * If the team is going to keep working on the project after the hackathon ends but the startup/business/third-party isn't interested, the project will be unfinished/dead/terminated for the company and the team will be encouraged to work on something else.

</details>
