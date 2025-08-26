# Project Agora

> From [Wikipedia](https://en.wikipedia.org/wiki/Agora): The agora was a central public space in ancient Greek city-states. The literal meaning of the word "agora" is "gathering place" or "assembly".

This ancient place aligns with the vision of this project: a beautiful, central place for our stakeholders to find everything they need and make the most out of their conference. Project Agora makes for a fitting codename while the project is in development.

## Context

The YMCA Center for Youth Voice is a department within the YMCA of the North (the YMCA association serving the Minnesota Twin Cities metro- and near-metro area) that is dedicated to preserving Minnesota's strong civic culture by helping young people understand systems of government and how to effectively use their voice to take action on issues that matter to them—because democracy must be learned by each generation.

The flagship programs of CYV take the conference form factor, with two separate programs:

**Youth in Government** is truly the flagship of CYV and was the first to exist, having been in Minnesota for 78 years. It is part of a national **Youth and Government** (YG) movement of the YMCA that provide similar experiences in nearly 40 states. In Minnesota, YMCA Youth in Government convenes ~1,400 8–12 graders from across the state to hold a large-scale model of the state government. Each young person is placed in a role in the Minnesota state government, be it in the legislature, courts, executive branch, media, lobbyists, or a more abstract 'National Issues Forum'. YIG is a four-day, three-night conference held mainly at the Hilton Minneapolis in Downtown Minneapolis and at the Capitol Complex in St. Paul, including the Minnesota State Capitol building, the Minnesota Judicial Center, the Minnesota Senate Building, and the Minnesota State Office Building. In addition to its ~1,400 youth participants, the conference relies on ~300 adult volunteers and paid staff for logistics, programming, delegation direction, safety, transportation, and more. The conference always happens in the first or second week of January.

**Model United Nations** is a conference in the same vein as YIG, running a model of the supranational United Nations. The conference is smaller at ~800 participants, with program areas including the Secretary General's Office, General Assembly, Security Council, Economic and Financial Council, Human Rights Council, and the International Court of Justice. Delegates select a country to represent and work within the organs to advance their country's and the world's interests. The conference is held at the Marriott City Center in Downtown Minneapolis, usually in the first week of April.

## The Need and Opportunity

Both YIG and MUN need ways to disseminate information, manage schedules, track program area materials, communicate, and more. Each conference always has a session book with schedules, room lists, rules, a directory, maps, and key information for all participants. This information is also shared digitally using a service called Yapp. Yapp allows organizers at CYV to add this information, often as files or links to other services, as well as schedule events and live announcements to the whole conference, to a single place accessible on a phone and from the web. Unfortunately, Yapp is quite limited in its functionality and repeatedly proves to be clunky and inefficient. CYV, and its peers throughout the YG movement, struggle to find a SaaS option for this use case that is: free or affordable, polished, easy-to-use, fast, and covers all use cases.

CYV also relies heavily on Airtable for its operations. It imports registrants and registration information from Y of the North's Salesforce and then uses Airtable for all conference functions: tracking participants, advisors, delegations, schedules, materials and material submissions, program assignments, rooming lists, and more. While Airtable proves invaluable internally for its UI, ease of use, and functionality, its integrations externally, to provide vital data to the wider conference, are limited. Airtable views and interfaces can't offer the seamless functionality of a purpose-built app or website for presenting things like schedules, program materials, etc. that are essential for each individual delegate or adult to know. Airtable has many integrations, but its API is also limited. Airtable remains excellent for its use case, but it leaves a need, and an opportunity, for more.

CYV and its national peers, continue to look for a perfect tool for their needs, but it proves challenging. What is presented is an opportunity and need for a purpose built, custom solution built from the ground up specifically for YG conferences.

## Core Features

These features are top priorities that must be implemented before the product could be released—they would be necessary to replace and improve on Yapp in a meaningful way.

### A personalized, accurate schedule built for each user.

Currently, schedules for CYV conferences are complicated and can be hard to read. Every program area has its own schedules and complexities. 

Using YIG as an example, a delegate in the legislature will have a different schedule than a delegate in the courts. Even within the legislature, there are different committees and legislative bodies, all in different rooms with different people. At YIG, there are three 'sets' of legislatures (a house and a senate), two for 9th and 10th graders, programming out of the hotel, and one for 11th and 12th graders, programming out of the Capitol. All will have different committees, different rooms, different mealtimes, and even different convocation times. To know when and where to go during committee time on the first day of conference, a 9th grader in the legislature will have to know a) which larger legislative body they are in (it could be the Myers House or Spear Senate, or the Humphrey House or Smith Senate), b) which committee they are in (could be one of seven), c) what time that set of legislature begins committee time, and THEN look up d) the room their committee is meeting. While paper and Yapp do their best to help, there is still a layer of complexity and confusion that can slow delegates down and cause real logistical challenges that hamper the experience.

The product will know information about the user—their grade, program area, committee or organ, etc.—and be able to show them their exact schedule: where to go and when, built just for them. It will surface relevant information when needed: five minutes before the end of a meeting, it'll tell them where to go next. In the morning, it will give them a look ahead at their day. This developer would draw parallels to Disney's Genie service that builds schedules for parkgoers at Disneyland and Walt Disney World.

### A contextual information depot for all things conference.

Yapp and conference session books contain vital information about the conference. It has maps of the hotels, the Capitol complex (for YIG), of the skyways. It has lists of meeting spaces, it has lists of places open during mealtimes. It has the Code of Conduct, emergency procedures, and the rules and procedure for the legislature, or organ, or program area a delegate is in. It has delegate and advisor directories, plugs for other programs, donation links.

In Yapp, these are often files that need to be downloaded to the local device before they can be viewed, or they're links that open in Google Drive or Airtable or some other platform. In session books, they're pages that need to be found and flipped to.

The product will have all of these data, well organized, searchable, responsive, and beautiful, all in one place. It will automatically surface whatever the user may need when they need it—working with their schedule. On the first day of conference, as delegations arrive, it will display luggage storage locations for the user's delegation automatically, so they don't have to worry about finding the sign for where to stow luggage while rooms are prepared. When opening ceremony adjourns, it'll surface a map for the user's first meeting of the conference. When their program area adjourns for lunch, it'll remind them of places to eat. The information presents itself in a way that is intelligent and useful when it is needed.

### A direct line of communication to the whole conference.

Yapp, in conjunction with CYV's use of Slack at conference, serves as a vital communication tool that can push updates out to the whole conference at once.

The product will deliver these announcements to all users at once if they're online. Announcements can be edited, multimedia, and formatted.

## Stretch Features

These features are not required in the core feature set before release. They are features that would greatly improve the conference experience and are "nice to haves" and, as the codebase grows, they should be kept in mind and added to roadmap if not implemented immediately.

### A hub for documents and program area materials.

In YG programs, participants almost always submit and rely on some form of document or material that they use during the conference. At YIG, legislators submit bills that they debate and pass, attorneys submit court briefs, lobbyists submit agendas, et cetera. At MUN, they submit status reports and position papers. At one of YG's national conferences, the Conference on National Affairs, they submit proposals. These materials play a key role in the conference experience.

Currently, to submit their materials for CYV conferences, participants fill out an Airtable form for their program area and select their name as a linked record to connect their information. Adding a submission feature would offer a more integrated and polished experience and move towards more cohesion between data platforms. Additionally, a place in the product to quickly and easily read the user's OWN submission would prove helpful when on the spot on the floor or discussing their material, without them having to pull up Airtable or dig through their own files.

To view materials from other delegates, participants currently have to dig through several pages in Yapp to find their program area, then scroll through Airtable or Google Drive, neither of which are optimized for quick and easy viewing on a mobile device. The alternative is to flip through a provided bill/proposal/material book, which a) incurs a cost to print and b) can be timely and slow to find the right page. Adding a feature that would surface the relevant materials for the user's use case (e.g. the bills in their committee when in committee and bills passed to the floor when on the floor; the resolution up for debate in their GA) natively within the app would contribute to a more integrated experience and improve the conference experience overall.

To track materials through the conference, participants have to rely on Airtable views (linked from Yapp individually for each program area group) or on a spreadsheet, which may not be frequently updated, slow to load and not mobile-optimized. Integrating the entire document tracking process into the product, so student leaders can update in real time the bills or materials they are discussing, automatically surfacing them to the participants in that group, and allowing the entire conference to track and read a material in one place, would contribute to a more integrated experience and improve the conference experience overall.

### An extensible, reusable conference experience platform.

The ideal end-product is not one that is hard-coded for each individual conference—that is, the features and data for each conference can be swapped out for another conference when needed. The same product can be used for YIG and MUN and the Conference on National Affairs and CYV's peers across the country. The branding could change, the data could change, the users could change, but YG conferences will generally have a need for all of the core features, which can be adapted or built differently with small adjustments for content-related differences. This developer envisions the final form of the product, when first produced or in the future, as a SaaS product purpose-built for the entire YG movement, not just CYV's YIG or MUN.

## Concepts of a Feature

These features have come to this developer as theoretical and conceptual inklings for features that could have a spot on roadmap much further down that road. This section may be updated as this developer continues to ideate and imagine.

### An integrated media platform.

At CYV and YG conferences, a media program area often reports on the conference goings on through multimedia reporting—online news, social media, broadcast, radio, print, and more. These channels can be scattered—across social media platforms, blogs, podcasting apps, and more—and integrating them into the conference product where participants already get all of their other information could lead to more engagement and a better integrated experience.

### A one-stop philanthropic shop, built in.

CYV conferences feature a student-led fundraising campaign called whYIGive, where participants can donate small amounts of money to CYV's scholarship fund and receive thank-you gifts in exchange: gavel-shaped pencils, whYIGive stickers, exclusive lanyards, or an entry to win an enormous stuffed mascot. The campaign is historically cash-only save for a Venmo account for online donations. Two roadblocks slow students from donating: not having cash, or not having Venmo. While tap and chip contactless readers remain an option, the ability to donate in-app using your platform's native digital wallet (Apple or Google Pay) and show a receipt to receive a gift would eliminate most blocks and encourage more students to donate.

### Native feature implementation.

On iOS, maybe Live Activities as a persistent schedule for the user, or local LLMs for generated summaries.

# Tech Stack & Development

Now comes the hard part. Designing and developing a service that can scale is a large task that normally takes a team of people. This developer is one person. Here's an early look at the technical requirements and stack for actually building the product.

## Specs & Requirements

The product would be available both on the web, from a computer, and on mobile devices across Apple operating systems and Android, especially phones.

The product would present information for the whole conference to anyone without being signed in, and deliver a personalized experience for logged-in users.

The product would be able to deliver core functions, like schedules and static information, offline as internet in conference environments is unreliable.

The product would be fast and responsive, regardless of the user's device's processing power or their internet connection. It should react instantly and natively.

The product would be secure and simple to sign in to—users have enough accounts as it is, and they trust us to keep their data private.

The product would be minimal and well-designed—just because it's deployed by an amateur team, it shouldn't feel like an amateur product.

The product would be branded to the conference and YG movement—the YMCA's font, logomark, and brand shapes can be felt throughout the product.

## Early Tech Stack

This space tracks developments and potential ideas for implementation.

Potentially using **PostgreSQL** as the relational database; familiar to Airtable but scalable and industry-standard. Maybe use Supabase for cloud.

Potentially using **React** and **React Native** for app if all features are supported and can look nice.

**One code base,** ideally. Flutter? Could also use native development, like Swift and SwiftUI for iOS and Kotlin for Android, but less ideal and harder to maintain.

**PWA** for web users—where to host?

Magic Link, or Sign in with Google/Apple for easy auth

hmmmmmmmmm

Backend needed.

Design in Figma? Whatever design is, needs to support Cachet Pro custom fonts; triangle and chevron custom shapes, and Y colors without being crowded or too dated.