# SCRF Interviews | Resilient Treasury Management - Daniel Ospina and Darcy Allen (Ep. 6)

The [Smart Contract Research Forum](https://www.smartcontractresearch.org/) (SCRF) has created a transcript of “SCRF Interviews | Resilient Treasury Management - Daniel Ospina and Darcy Allen (Ep. 6)”. For more information about the podcast, please click here,

_This transcript was generated using the video version. The audio version timestamps are -7 seconds._

**Eugene Leventhal:**

**[00:13]** Hello and welcome to the SCRF Interviews podcast. I'm your co-host for the day, Eugene Leventhal, and today's topic that we're going to be getting into with our other co-hosts and our esteemed guests will be - protecting the heart asset, making a DAO and its treasury robust against attack. So to kick us off, Kelsey, who's our other co-host for today, Kelsey Nabben from RMIT, do you mind just jumping in and giving a quick intro?

**Kelsey Nabben:**

**[00:36]** Sure, thank you, Eugene, and thanks for having us. My name is Kelsey Nabben. I'm a researcher at the RMIT Blockchain Innovation Hub. And I'm really excited for this conversation. My research is on resilience in decentralized technology, including DAOs. But I'm looking forward to hearing what my colleague, academic and what industry practitioner, Daniel has to say today. Daniel, would you like to introduce yourself?

**Daniel Ospina:**

**[00:59]** Sure. Thank you. Thank you very much for having me. I’m very excited about this conversation. From my side, I'm a DAO practitioner. I specialize in governance and organization design. I come from a background [of] studying and consulting and essentially working on figuring out what networked organizations are and how they could operate. And then I guess it was only a matter of time before encountering blockchain and realizing that this is the space where we have both the funds, the technological capabilities, and a desire to innovate and do things differently and I became fascinated about this space.

**Daniel Ospina:**

**[01:42]** My most recent engagement was with Aragon to help them with facilitating the process of designing and launching the Aragon network DAO. Now, I'm in the process of speaking with different organizations and so on, and perhaps launching a DAO tooling studio as a next step. So thank you for having me.

**Eugene Leventhal:**

**[02:03]** Great, thank you, Daniel and Darcy, do you mind jumping in?

**Darcy Allen:**

**[02:06]** Fantastic. It's great to be here. Thank you for having me. My name is Darcy Allen. I am an academic economist, a senior research fellow at the RMIT Blockchain Innovation Hub. I started my academic career as an innovation economist, five or six years ago, working on the institutions and the governance of innovation and then came across blockchain and crypto, got completely obsessed with it, and now we have a research center that focuses on blockchain technology from a social science perspective. I try to take the tools of economics, of political science, of political economy and apply them to the sort of cutting-edge problems that are facing the industry today. 

**Darcy Allen:**

**[02:53]** So I hope what I tell you I'm working on today, I'm working on something very different in three months, whatever the big issues are at that time. So we try to stay super relevant and, I guess, pivot to whatever problems they are facing and see what we can add as academics. So, it's great to be here and I look forward to the discussion.

**Eugene Leventhal:**

**[03:14]** And we really appreciate all of you joining. Before we delve into sort of the depth of how to make DAOs robust against attacks, I wanted to start with the question of what problem treasury governance is trying to solve in the first place, to really set the stage for the rest of the conversation. So, yeah, Darcy or Daniel, do you mind jumping in on that one?

**Darcy Allen:**

**[03:39]** I'll jump in on this one. I think there's multiple problems, and I think this is a little bit misunderstood. We can get very focused on one particular problem that we're facing at that time in treasury governance, whatever it is, whether it's diversification or maybe there was a hack or whatever it happens to be. But if I guess we zoom out a little bit, I think there are two main problems that the treasury's face.

**Darcy Allen:**

**[04:03]** The first one is what an economist would call a knowledge problem, and that's the problem that any decision we make about a treasury happens under uncertainty. We don't know what we should spend the treasury on. Should we spend it on ecosystem incentives, or should we be spending it on research? That's a knowledge problem. We don't know how to solve that. And on the other hand, there's sort of an incentive problem or an opportunism problem. How do we know that the treasury is being spent well? However, that's defined. I think we'll dig into this a little bit.

**Darcy Allen:**

**[04:42]** But that's the problem, that all of the stakeholders within a blockchain ecosystem, as broad as they are, have to have some trust that the treasury isn't being misappropriated for various purposes, and that there aren't people seeking too many rents out of it or that it's vulnerable to attack. So, there's sort of these two problems: there's a knowledge problem - what do we do under uncertainty? And there's an incentive problem and an opportunism problem: how do we make sure it's safe and secure? And any governance structures we try and put into a treasury have to deal with those problems, and sometimes they're conflicting. So, I think it's really difficult to work through those challenges.

**Daniel Ospina:**

**[05:26] **That resonates a lot and thank you for saying that. For me, there is also something I would add like building on top of it, and this very much relates to the knowledge problem that you're talking about, that is perhaps a very unique characteristic of DAOs compared to other treasuries, is that because there is so little central control, and we have so few tools for sense making and decision making collectively and sometimes not even an intention to have that. 

**Daniel Ospina:**

**[05:59]** So, there is a whole range of DAOs being anywhere between a company and a public goods and so on. It's not only in a company that you can be well, if we're increasing value for shareholders, that's a good decision. So at least the parameters to know what good decisions are, or bad decisions are, are more or less clear in the traditional world and in DAOs all of those pieces are thrown up in the air again and easier to see, and every organization kind of needs to negotiate that again from zero, which ends up being deep philosophical question.

**Daniel Ospina:**

**[06:33]** So there is also kind of, let's say combined with an infrastructure problem, a tooling problem of “how can we address these other problems”? But it's more to say that this is a brutal space with a lot of challenges, a lot of uncertainty, trying to deal with large groups of people with semi-anonymity, sometimes permissionless and so on. That why these knowledge problems, these incentive problems are particularly tricky to address.

**Darcy Allen:**

**[07:06]** I think that's exactly right, and I think it's hard in part because we don't really know what blockchains are. So sometimes they kind of look like firms: they're trying to achieve a particular objective, we're trying to do it all together. Sometimes they look like markets: there can be payments within them and so on, and sometimes they look like governments: we talk about these treasuries sometimes as if it's a public purse or a treasury and reconciling those objectives can be really, really hard. We don't even necessarily know what the objective of the problem is that we're solving, and that problem changes as a blockchain ecosystem grows. 

**Darcy Allen:**

**[07:49]** So the problem on day one, when you're deciding to structure your DAO and get your very first distribution of tokens, is very different to when you've got a multi-billion-dollar market cap, and now you have so many more stakeholders, you've got VC’s who want particular things. You've got people buying governance tokens on a secondary market and coming in and voting for things.

**Darcy Allen:**

**[08:14]** So just to add to your point, I completely agree. And I think we're still in the stage where we're trying to find out what this weird new technology is. The tools, as you say, are super important in working this out. 

**Kelsey Nabben:**

**[08:30]** So, I'm really interested to ground this in some practice, and I'm looking forward to kind of jumping between the theory and the practical applications. What are some of the threats to DAOs? And I guess the way that I'm thinking about this question is that blockchains and DAOs are both socio-technical organizations. So, you guys have each touched on some social threats and some technical threats in your broad definition of the governance of treasuries here, as well as those kinds of threats. How can they either be negative or positive? How can they provide the opportunity for adaptability and improvement? And maybe Daniel it would be interesting to hear from you to start with in terms of when you engaged with Aragon, what were some of the things you were thinking to design for or against?

**Daniel Ospina:**

**[09:26]** In this instance, Aragon was a peculiar case, in the sense that they had been previously more decentralized, then they re-centralized, and this was another attempt at decentralizing in a more effective way. Historically, what had happened, and they had more of a network of DAOs or a network of organizations rather than a direct to contributor DAO. The terminology is perhaps a little bit fuzzy, but essentially, they were giving grants to these multiple centralized organizations that were developing different things for the Aragon network.

**Daniel Ospina:**

**[10:07]** And that had some issues for a wide range of reasons, some of which I just don't know because it was back in the day. But on this occasion, the division I was putting forward was more of a DAO where contributors could directly add value and then over time, evolving to having multiple teams, so sort of like teams of teams set up. Very liquid with fairly decentralized governance. Thinking on that setup, some of the challenges are and also Aragon being an organization that's been around for a while, there is a lot of the treasures out there in the wild.

**Daniel Ospina:**

**[10:48]** There is some early-stage wealthy investors, they were the founders, who were not really involved and had significant token. So, essentially, we had huge disproportionate holding of tokens. So, there would be a few people who could swing votes and almost make the network follow their will to some degree. And it was important to find ways to balance that out with a newer, engaged community, who had relatively limited token holding. So essentially, it was kind of like designing for an organization where you need to empower people who have to make decisions, who have very small amounts of tokens, while at the same time being mindful that maybe someone gets a huge fund.

**Daniel Ospina:**

**[11:30]** I had some anonymous people reach out to me and say, like, “Hey, I want to buy 1 million tokens under the counter. Is there someone I can speak with in private?” and I'm like: “No thank you.” But that was happening and that's the sort of environment that we're in. So that was one of the key design criteria: can we offer safety while having very low thresholds?

**Daniel Ospina:**

**[11:53]** The other design principle was this is going to start “very M.V.P.”, very rough. We just want to get it out extremely quickly. And that was just a requirement that was put to me by the Aragon leadership. He was saying “we want to have a DAO in three months”, and I'm like, that's kind of nuts, but okay, let's try. And it can work but obviously you made tradeoffs at that point. And so, the idea is, it's what I'm calling a sandbox approach as opposed to training wheels.

**Daniel Ospina:**

**[12:25]** So instead of simulating the situation by keeping a lot of control. It's more like get it out, even if it's not perfect, and let the community start iterating it. Which also meant all the thresholds and all the systems. So, we needed to be able to change the governance process itself. It should be very easy to iterate it. And then that obviously brings all the other issues of - there is a large community out there who has no clue what we're doing here, they've been disengaged for a long time and so on.

**Daniel Ospina:**

**[12:58]** So there were very strong issues around these knowledge problems and also a very peculiar situation where Aragon, the last time I checked, it was valued at about USD150 million market cap, but the value of the treasury exceeded the USD 300 million. So, there could be some controversial situation there or maybe some of the community didn't believe in the project anymore or generally the market was undervaluing the project extremely. So that could kind of create incentives for people to try to withdraw their funds from the projects. While the project lies in this strange limbo of trying to be a corporate or a company in a culture of company execution and style, and those sorts of objectives.

**Daniel Ospina:**

**[13:50]** And then on the other side, a very big mission, like pro-social mission that he's trying to achieve. So, in the past, like in the previous time they tried to decentralize, the issue was that people were asking for funds for like: “we want to go and do exploration in Mars.” And maybe that could be argued that it serves the mission, because the mission is very broad and big, but it was clearly completely left field and really not what anyone initially had intended. So, he was trying to find ways to figure that out.

**Kelsey Nabben:**

**[14:23]** Yeah, that's interesting, so you're talking more about actually the social dynamics of governance as both an opportunity and a threat in DAOs and to DAO treasuries. Darcy, what are your perspectives on the threats to DAO treasuries?

**Darcy Allen:**

**[14:39]** Again, and** **I said this with the first question, I think it's really easy to focus too much on the given threat that you have at this time. What we like to do is we'd like to take frameworks that we have elsewhere and apply them to new areas, and one of the frameworks that some of my colleagues and I have talked about, is in a field called new comparative economics. And the basis of this field is, when you think about problems that you're facing in an economic sense, you can think about different governance structures as minimizing two types of costs.

**Darcy Allen:**

**[15:16]** On the one hand - we have in treasuries; we have insider costs. We have the costs of the founders of a multi-sig or the board members of a foundation, who might somehow misappropriate the treasury, send it to their friends, run away with it and so on and so forth. They are the insider threats that come when you create positions of privilege over the treasury itself. When you have a multi-sig, or you have a foundation that's controlling the treasury.

**Darcy Allen:**

**[15:54]** Now, on the other hand, though, you've got outsider costs. Those are the costs that outsiders might come in and buy governance tokens, for instance, and stack some vote. They might undertake some sort of Sybil attack to use the voting system to their advantage and siphon off some of the treasury. And whenever we're thinking about the way that we govern the treasury, you've got to trade-off between either insider costs or outsider costs. And every different governance institution that you put in moves you in one of those directions.

**Darcy Allen:**

**[16:33]** So if you have a treasury that's controlled just by an individual, not even a multi-sig, it's all insider costs. You're worried that they're going to run away with the treasury or do whatever they like with it. If you move from there to a multi-sig or to a foundation, or to an elected foundation, you're moving away from the threat that those specific individuals will attack the treasury. But you're raising the costs that outsiders might come in in some way and try to take the treasury for themselves. 

**Darcy Allen:**

**[17:10]** So there's sort of this basic trade-off right now. When we think about this, it's important to understand that, as I said before, those costs change over the life of a blockchain ecosystem. In the very early stages, you might face a really big threat from outsiders coming in and stacking a vote when there's just a low voter turnout; for instance, there might not be that many tokens in circulation. In that circumstance it might make sense to actually have it held with the founders in a multi-sig. But, as you move along, you might decide to decentralize your governance of a treasury, because there are more stakeholders, because the optimum governance structure is actually more decentralized.

**Darcy Allen:**

**[18:00]** And the way that all of these tools, that Daniel was mentioning, fit in, is that blockchains enable us to create new tools to minimize these costs in different ways. So, we obviously get new types of voting, like quadratic voting. That is an attempt effectively to reduce the outsider costs of large token holders coming in and affecting the vote. We're creating these new governance structures to minimize those costs in different ways.

**Kelsey Nabben:**

**[18:32]** Yeah, that's so interesting that you mention it, because then you have tradeoffs. Obviously, the Sybil attack issue becomes a real possibility in terms of a threat vector because people are incentivized to create multiple fake identities. So, I like that way of framing it as this constant sort of thing around tradeoffs to solve knowledge and incentive problems.

**Darcy Allen:**

**[18:56]** Yeah, there's this constant trade off and both of these costs are unavoidable. In any governance structure you implement for a treasury, you're going to face some insider costs and some outsider costs. And the question is where do you want to place yourself? Do you want to place yourself in everything goes out to a DAO vote and it's automatically executed, and we see what happens? Lots of disorder costs. Or do you just want the founder to have their own, to control the treasury completely?

**Darcy Allen:**

**[19:27]** What's interesting, particularly about what Daniel was saying, was we also discover what those costs are over time. For instance, in SushiSwap, we didn't realize that there was a threat that Chef Nomi would run away with the Treasury. Then it happened and we went: “Oh wait. Maybe we're not in the right spot here. Maybe we should decentralize this to a multi-sig or whatever.” But, the point is, you figure these out over time. And as Daniel was saying, the way that you figure them out, is you effectively ship that DAO, and you see what happens when it's out there or whatever the governance structure is. And they stress that too, but you learn.

**Daniel Ospina:**

**[20:13]** I quite like the framework of having this polarity that I could almost say, the cost of risk of centralization versus risk of decentralization to bring it to DAO terminology.  And then, I would maybe add that, it occurred to me that the other polarity is between safety and risk taking. So, between, let's empower the community, especially if we think about DAOs, we want to make it as easy as possible for the community to be able to participate and contribute. And one issue adjacent to the whole treasury risk management conversation, is the voter participation or voter apathy and so on, but just to point that that's an issue.

**Daniel Ospina:**

**[21:05]** And if we had a lot of safety, then that's the tradeoff as well. So, we kind of need to figure out between these things, how much is safe enough and what are we having to do to make it safer? If we had a lot of mechanisms, a lot of delays, higher thresholds whatever it is, whether it's more protecting against insider cost or about outsider cost, then we'll also have to calibrate that other bit according to how much risk we want to take and how much we want to learn quickly and iterate and improve based on that.

**Darcy Allen:**

**[21:42]** And as you're saying, it's not just what you want, it's what the whole community wants. Ironically, we're throwing things out to a DAO vote to find out what their feelings are about how it's governed, and there's this odd feedback loop. There's obviously this decentralization ethos surrounding all this and that has to be taken into account of which point you pick in that governance, which is tough. You don't always know what the community wants and the community changes as you grow, which is a challenge.

**Daniel Ospina:**

**[22:21]** The thing that cannot be stressed enough, that is not to judge where the DAOs should go, again what's right and wrong? It really should be from the community aspect, which is this changing entity that a single individual never fully knows. We rely on the governance mechanism to learn what we want because we cannot just know it ourselves by introspection like a traditional founder would. And I think many DAO projects confuse that and start stressing out and being like “Oh, but I'm not sure about that decision” and “that's an issue, that's an attack.” No, it's just different from what you were thinking. But it might be more aligned with the community. You don't know that yet. Let it go through instead of trying to stamp on it, in the early stage for example.

**Kelsey Nabben:**

**[23:11]** Yeah, lots of thoughts off the back of your comments. Darcy, you suggest that polycentricity is an approach to making a treasury more robust. Can you explain what this means and where it comes from and then identify how decisions or objectives can be set by the community within a polycentric organization?

**Darcy Allen:**

**[23:38]** That's a massive question, but it's great. From an academic perspective, polycentricity is a theoretical construct that describes a system that has many centers of decision making. And that's in contrast to a monocentric system, which has one center of decision making. A lot of the research on polycentricity focused on some of the early work by Elinor Ostrom and Vincent Ostrom, who are economists and political scientists, focused on the problem of metropolitan policing.

**Darcy Allen:**

**[24:14]** Now, this sounds a little bit obscure, but we'll bring it back to treasuries in a second. The problem at the time was that you had lots of different centers of little police departments, and this looked really inefficient. It looked like they were overlapping, there was no centralized administration and there was a push to move all of these into one big, monocentric, system of governance. The polycentricity looked messy, and it didn't look like it was producing any value. And there was a lot of failed work that showed that there are actually a huge amount of benefits of having lower levels of decision making that can make their own decisions on the ground with local knowledge. They're more adaptable. They understand their local context a lot more.

**Darcy Allen:**

**[25:06]** Bringing this back to blockchains and treasuries. At the moment, I think this is changing, but a lot of treasuries are governed in a way that we just use one type of decision making for the treasury. We put everything out to a vote, or we put everything to a committee, or we just pick one type of governance structure, and we go with that. Now, there's a few issues with that, and I think it opens up a lot of attack vectors when you've got one central point of decision making.

**Darcy Allen:**

**[25:40]** The benefit of saying, “okay let's make many centers of decision making.” So, let's have a smaller grants body that's just doing this particular type of grants. Now we have this other committee that's working on ecosystem incentives. This is another group that's elected and working on something else. What you've got is you've got many different centers of decision making that are all kind of specializing in their particular area. Now this can look like bureaucracy, and it also looks a little bit like centralization and hierarchy within a blockchain, and communities can have issues with this,

**Darcy Allen:**

**[26:20]** But there's value in having a more polycentric system. There isn't one central voting system that can be attacked, for instance, in a Sybil attack or something else. There's lots of different systems. And what you get is a lot of discovery and learning about what those different governance structures should be. Some of them will fail. Some of them won't work very well. We'll figure out that that committee is completely dysfunctional and disband that and so on. But I'm a big fan of polycentricity as a guiding principle, so not trying to do a one size-fits-all governance structure and moving towards a more polycentric system. The community might not like it though.

**Daniel Ospina:**

**[27:10]** I couldn't agree more. I was trying to work with a few of those principles for this last week, in a DAO project and stuff, and one of the ideas that we've been talking about, and now in ecosystem I'm seeing, gaining more momentum and more and more people are engaging in the conversation and the idea of sub DAOs, which are kind of like DAOs within a DAO.

**Daniel Ospina:**

**[27:37]** Now the conversation also suffers from the lack of definitions around DAOs itself, so sometimes a sub-DAO is a committee, sometimes a sub-DAO is some community-oriented voting mechanism. But that's a whole point, different decision-making strategy: different governance systems that collaborate with each other. But there is indeed an educational problem with the community, I did encounter some resistance from people, quoting from “simplicity is the best answer” or any sort of meme that talks about simplicity.

**Daniel Ospina:**

**[28:15]** There was a subset of the community that really liked this, and they were like, “Oh, but this is very complicated.” Well, it's true that once you have multiple centers of decision making, anyone is going to have to try to find the ideal one for their specific use case, and if they need to learn about three or four, that's a lot more complicated than one process for one. But, that being said, I still see a lot of benefits. I guess it's about finding the right balance on when to introduce it; maybe perhaps starting with, two, so, the idea is baked in since the beginning and then adding more as one goes along and really, really working on the educational onboarding piece to make sure that this is kind of like functional and people can navigate the DAO, navigate the network, but I see tremendous benefits for it.  

**Daniel Ospina:**

**[29:13]** Even in the terms of cycles, if nothing else, like the length of time it takes one to ask for a huge sum of money, that requires a lot of thinking and time. But if one needs, I don't know, $200 to pay some gas fees, well, that shouldn't take you having to write a three-page proposal. But, if you're asking for a million from the treasury, well, yeah, probably a three-page proposal is the minimum with community feedback and grants.

**Darcy Allen:**

**[29:43]** Community feedback is a very good point.** **The question then is: if we're starting from a more monocentric system, there is one system of governance, how do we get to a more polycentric system? And the challenge with most polycentric systems that work is that they're not designed. So, there are systems that have emerged as polycentric systems and then eventually humans come in and go “Oh, this looks messy and complicated.” Let's, as you say, “let's simplify it, that's all too complex.”

**Darcy Allen:**

**[30:15]** The problem is that most of them started polycentric, and then there's a push to centralize them. And I don't really know how we overcome that, except for, as you're saying that, that education piece. So, there's a field in political economy called robust political economy. What it says is that, if we're trying to design a system, let's start from some realistic assumptions rather than some unrealistic assumptions. Let's assume that people don't know everything. So, let's assume that humans are bounded rational, and they face uncertainty, and we're not sure what to do; we have a knowledge problem. 

**Darcy Allen:**

**[30:59]** And let's also assume that people aren't always good people. They're not always benevolent, they will act in a self-interested way sometimes, they will be opportunistic. In that circumstance, what kind of institutional system do you create to deal with those dual problems? The reality of the world - there's uncertainty and there's all these incentive problems and people can act poorly. That literature basically comes back to - enable polycentric systems to emerge. So, you have a minimum set of overarching rules, think of it as a constitution, I guess, that is designed in a way that enables centers of decision making to emerge within it. 

**Darcy Allen:**

**[31:49]** And in this story, what happens is: that's how you get a robust system. If there are feedback loops, as you mentioned, which is a really key part of this story, then you're trying to design a rule system that enables other rule systems to emerge within it.

And this is probably getting away from what Kelsey wanted, which is maybe a little bit too academic. But you're designing for that problem of how do we evolve our governance structures when we don't know what we're doing and there's bad people?

And I think it kind of all comes back to that in the end, and that's how you get a robust system.

**Kelsey Nabben:**

**[32:31]** Yeah, this is phenomenal, and the empirical research completely backs that up, in the sense of there are these massive projects with huge treasuries that are having this issue of kind of re-decentralizing, as Daniel said. They decentralized and then freaked out because that wasn't really working and then re-centralized and tried to plan again on how to give governance power back to the community. But this idea of working at multiple scales and integrating feedback loops makes complete sense, and some projects are working with it. 

**Kelsey Nabben:**

**[33:10]** Examples that come to my mind are the Lido LEGO grants program. That's super light for under a certain threshold of money that they grant and have a wish list. And then another case study that I was really involved in is Gitcoin and looking at how they've evolved some of their sort of steward working groups to become specialists in their area. But that idea, you said Darcy, about a constitution or the kind of terms and conditions guiding the kind of norms and cultural values of a DAO, I think is really important. And I'm curious to hear from both of you, because you wouldn't normally think of robust treasury management as coming back to the constitutional principles of a DAO, but that seems to have sort of been in the loop that we've gone in the conversation. Eugene, did you want to add to that?

**Eugene Leventhal:**

**[34:08]** I wanted to add a slightly different angle on it just in terms of, a lot of what has been said throughout this conversation in general touches on some challenges that might be specific to this space, some broad challenges around humans collaborating together and then some very open-ended questions around “how do humans manage ambiguity better? How do you design systems that allow for emergent behavior?” These are kinds of questions that I don't think anyone has a good answer to that works in all environments yet and the whole idea of you need to focus on what's right for your ecosystem.

**Eugene Leventhal:**

**[34:45]** And that just makes me wonder, if any of you were in the position of tomorrow you're in the situation where you now need to fully, soup to nuts figure out the treasury structure, the governance structure and plan out a new kind of protocol. Not to ask the moot point of giving us the best practices because I think that's a self-defeating question. But at least what would be an element of the mindset that you think is so important when thinking of these kinds of systems?

**Eugene Leventhal:**

**[35:12]** Because even just as simple as, if you’re designing it and in the token economics and what was mentioned about what happens at the concentration of the early airdrop recipients a lot of the time, but you inherently have to come in with this mindset of “Oh, I’m building something that I don’t get to control.” And that seems counterintuitive, at least in certain Western cultures. What are your thoughts on sort of the mindset of even thinking about these kinds of problems, given how many unknowns and points of complexity there are here?

**Daniel Ospina:**

**[35:45]** I'll jump in, trying to tie that up a bit with the concept of the Constitution as well, which I think the two can come really well together. If we're talking about trying to have a sort of foundational principles or foundational ideas that then will take their own life and people will make them their own and evolve in some ways. I would say, a few things that I encounter that work across multiple cases, one is thinking about the resources or multiple capitals, a little bit holistically.

**Daniel Ospina:**

**[36:24]** Some DAOs will have a very small treasury, but they might have a big community of engaged contributors. They may have essentially a lot of social capital within the community, a lot of knowledge capital, a lot of intellectual capital, but limited financial capital. And I think these are largely interchangeable and way more interchangeable in the DAO world than before. Perhaps because the market is more efficient, or perhaps because there is more speculation one can make.

**Daniel Ospina:**

**[36:52]** If you have a community, you can raise a lot of funds. If you raise a lot of funds, maybe you can do a huge airdrop and start to activate a community really quickly. Obviously, to make them a “real” community takes time. But anyway, it's more to say that there is this idea of not trying to zero in on the treasury as the only capital that one has but thinking about that holistically and then applying these other principles to all of them. That is enabling self-organization, at the same time that alignment mechanisms. 

**Daniel Ospina:**

**[37:28]** So I use a lighthouse metaphor in that, the lighthouse kind of shows you where the shore is, it kind of shows you where the rocks are, but the lighthouse doesn't tell you where each ship needs to go. Each ship is making their own directions, but they have this somewhat centralized mechanism that shares information with everyone to have a shared context of “Where is the shore and where is the sea? And I think that helps a lot, and the more one can create forums or spaces where people can exchange ideas and negotiate their worldviews, that can be regular community gatherings. That can be “let’s try to create a vision together.” The vision is not enforceable, but just the act of having those bridging mechanisms kind of really helps while at the same time finding how to enable self-organization.

**Daniel Ospina:**

**[38:22]** And I mentioned the capitals because in self-organization people can vote with their feet and they can join Team A or Team B or Team C, and they can change between those teams as they see fit. But it can also be, essentially the community can decide, whether they fund Team A or Team B, and sometimes funding is not about putting in the financial resources, it is just enabling people to work in one or the other. In other times, you actually need funding because people might be bootstrapping their own engagement through tokens and there will be no difference in between these two. 

**Daniel Ospina:**

**[38:57]** But that's why I think it's important to think holistically and allow some level of self-organization or essentially allow people to decide while having the broader alignment mechanisms. Perhaps the final thing that comes to my head is related to the complexity of the Constitution. There can be a lot of tension in between trying to create a constitution that is very comprehensive and protects a lot from different situations and then trying to adhere very well to the Constitution instead of taking it more as a loose, general sense making as a lighthouse essentially. One can try to take it more as the absolute rules.

**Daniel Ospina:**

**[39:47]** And I think the more the constitution can come close to a lighthouse, obviously, one needs clear rules, but the more the human readable part of it can be a lighthouse, and the ingrain mechanism design that is hardcoded in the blockchain and has no ambiguity. The more like the hard roles we can shift into the blockchain to let the blockchain do what he does really well, code is not ambiguous, let code be unambiguous and when we can allow ambiguity, let that be as much human readable as possible.

**Daniel Ospina:**

**[40:20]** Because otherwise there can be a lot of issues like, “but that's not what that interpretation should mean”. And before we realized, we end up with all the legal complexity that a lot of people are trying to escape away and you'd have loads of lawyers involved and these can quickly snowball into a disaster and become a cultural thing where every decision needs to be checked with their lawyers before anything happens, and then you lose all agility and your feedback loops become super long.

**Darcy Allen:**

**[40:52]** I find it very, very interesting, and I agree. I think the problem is who decides where the lighthouse is? So, in the very early stages of an ecosystem, there's a reason why constitutions and even a description of what a treasury is for, is just incredibly broad. It's just going to solve all the problems. It's going to fix everything in Web3. There's this broad idea of what a treasury does. And I think that's for a good reason. There's lots of uncertainty. But then we need some way to hone in on more specific problems as they arise.

**Darcy Allen:**

**[41:36]** So right now, we might be facing a massive scaling problem. The Constitution or whatever we initially said the treasury was for, we didn't know that this was going to be our problem this six months. So, the question is, then how do you create a system where that second objective can emerge as an objective? Now this sounds a little bit circular, but what this looks like to me is perhaps the community deciding, setting sort of new objective for a bucket of treasury funds saying: “We're just focusing on scaling.” And then what I would like to see is delegation of those funds to people with some discretionary use of them.

**Darcy Allen:**

**[42:19]** So maybe the community acts as a kind of a sovereign, if you will, that decides “here’s our objective for this round.” But then what you do is once the community is set on an objective, with that money you delegate it to people who can do whatever they want with it to try and achieve the objective. I don't know what they want to do with it. They might convert it straight to USDC, and everyone gets really angry. And then there's a bunch of different paths that they can go.

**Darcy Allen:**

**[42:50]** But if you have a feedback loop at the end and those entrepreneurs that have been delegated can try and achieve the objective, then you do bring it back to the community at the end. But I think you're exactly right that the lighthouse kind of needs to set these boundaries and then people need to have some freedom within them. It's just that changes over time, and it's not going to just sit in an initial constitution or an initial description of what a treasury should do. It's a very hard problem. I just wish there was more: we traded this more like an entrepreneurial problem that we're handing out cash to someone to just try and solve the problem quickly, and then we have feedback at the end; rather than everything being decided by everyone.

**Kelsey Nabben:**

**[43:41]** Yeah, it's so interesting, and what you've kind of described is sort of what Gitcoin looks like, but as a funding mechanism in the Ethereum community, that has gone through multiple iterations from The DAO, which was meant to be pure algorithmic governance and obviously suffered from a bug in the software code, to Ethereum foundation grants program to Ethereum community fund. And there's been all these fails, but lessons learned along the way. And then Gitcoin has kind of iterated and now transitioned to a DAO where you are seeing all of these buckets of money changing each round for all these different things, getting sort of donated to all these different teams. So that's actually quite interesting.

**Daniel Ospina:**

**[44:27]** I guess we're seeing a new evolution of that, that I think can really help this approach that you are mentioning. We have escrow mechanisms that are starting to come into effect. There are KPI options. So essentially different mechanism designs, there is even courts, like Clara, Celestia, Aragon Court and so on that can see, if plugged into one of these projects where that funds or initiatives, or a person or a small team that has gotten some funds delegated to them to try to solve a problem. These different mechanisms can help to mitigate the risk here. And so, I'm hoping that we see more and more of these approaches because historically there have been also these situations where someone asks for a grant and then they keep their money and disappear because they were anonymous and no one knows who they are. Or maybe they're not even anonymous, but they just don't deliver at all and keep the money. 

**Daniel Ospina:**

**[45:33]** With some mechanisms, I see both a fantastic opportunity to have more of these. Also, perhaps, the risk that people end up designing only for the situations where it has gone wrong. Instead, for the many situations where it went right, and you see a little bit at risk with escrow systems. It's like, oh no, there was one time someone ran away with funds so now let me make sure that everything is super regimented and so on. But if used properly, these mechanisms can add a lot of safety for contracting and so on and really enable the delegation of funds and perhaps more autonomy, while the objective at the end or even the objective initially is kept clear. 

**Daniel Ospina:**

**[46:14]** As long as this is really kept at the edges in small experiments, quick feedback loops. Because otherwise we end up a little bit in the waterfall approach of like, let's do loads of planning for a project that's going to last a year and halfway through that project we discovered that it was a terrible idea, and the objectives should have been completely different, and there is no room to iterate on this. So it's more like trying to leave the iteration very open objectives that can evolve very quickly, but then having the quick feedback loops to review all of that, to give some funding, experiment with a phase, see what happens, allow people to figure out their own strategies, their own way to invest these funds and then obviously across a portfolio of initiatives that are being invested in,

**Daniel Ospina:**

**[47:03]** If one of them turns sour or malicious, then you eliminate them and don't give them the next tranche of funding and continuing betting on the others. And taking more of a sort of risky investment approach, like a VC approach to treasury management, rather than a very tightly controlled, centrally planned, loads of pre-thinking, loads of long project, not mega project management but more like a VC approach to treasury management.

**Darcy Allen:**

**[47:34]** I completely agree with that approach. And I think it goes back to something that I mentioned earlier, which is we should try and learn from the real world as much as we can in this space. We've seen grants giving bodies and VCs for hundreds of years now. VCs are obviously solving a particular entrepreneurial problem that you have uncertainty about whether they're going to do the thing or not. Governments have this problem where they have all of this money, and they need to fund innovation and they've tried to solve that in many ways. Sometimes they use prizes, sometimes they use grants. They have a whole suite of tools that they deploy to try and deal with this fundamental problem that none of us really know what we're doing, but we need to hand out this money to get some sort of innovation or research or something good that we want. But we should design feedback mechanisms after the fact. And I think you are exactly right.

**Kelsey Nabben:**

**[48:35]** Yeah, I really like that, and you guys mentioned before just the point of experimenting with different types of mechanisms, so it's not a vote. Everyone votes so it's 100% pass, next question put to the entire community of hundreds of people, even if it's a specific topic area of things. I can see that polycentric approach sort of starting to apply.

**Kelsey Nabben:**

**[49:00]** Do either of you have any opinions on algorithms and their role in governance, in DAOs or treasury management as well. Daniel you just referred to kind of decentralized court mechanisms, and I've been keenly interested in this idea of who gets to design the algorithms and when are they an opportunity to remove an option for political coercion or centralization and control? Or when are they a potential threat in the sense that you can so effectively manage and monitor an online community that people have potentially strayed from the initial ideology or goals?

**Daniel Ospina:**

**[49:42]** I find the courts mechanisms to be really, interesting. At least the 3 that I know of that I was mentioning, Aragon Court, Celestia, and Clara are very similar. They all start with this shilling game idea, which is a relatively simple algorithm. The idea is basically people are incentivized to give their opinion. And if they agree, essentially if all three people are agreeing, then that's good, they all get rewarded. If one of them disagrees, they get penalized.

**Daniel Ospina:**

**[50:21]** And so what this forces is that instead of people saying this is what they think is best or this is what they think is right, they try to figure out what is the default interpretation? What are my peers most likely to understand and think in this situation?

So, it’s this very peculiar mechanism that allows to find what is the most likely consensus in a subjective situation? And so, there is a way to bring the human readable world, the ambiguous world into more objective terms and play with that. And so they compare well with like constitutions or with some sort of human readable agreements to then interpret - did the agreement actually meant that this decision is within the agreement or outside of the agreement that it's trying to depart?

**Daniel Ospina:**

**[51:14]** Now that as a theory works really well. In practice, it is really challenging. And these mechanisms are still quite early stages. I found personally, through direct experience, this is not research based or anything like that, but just my own observation, is that they work mostly as a psychological deterrent to attacks. Like if any attacker goes like, “well, there is a court, and now I have to put some collateral to put these proposals forward and the community might challenge it in court.” So, there is no point in me trying to just do a flash loan and try to get the community to transfer all their funds to me because there is a court mechanism that can stop it. 

**Daniel Ospina:**

**[52:02]** So in practice, they get used very little, very infrequently. But they are a safety mechanism. When they do actually come into effect and they actually need to that work, it's a little bit messy and it's a bit expensive and you probably require multiple rounds, and you end up bringing a lot of jurors together and so on to actually find these default interpretations. And then the jurors might be even very confused and so on, which I think is more to say that they are at a very early stage of development as tools, but they kind of protect against, let's say the 51% attacks and stuff like that. 

**Daniel Ospina:**

**[52:40]** So now coming back to the point on algorithms to this, I think this is a relatively simple algorithm. The majority gets rewarded, the minority gets penalized of the arbitrators, of the guardians, of the jurors in the court. So, these sort of relatively simple algorithms that are smartly used can add tremendous value in governance decisions. And I do envision a future where we can have more complex algorithms like AI/ML sort of things, neural networks coming in and helping with decision making and supporting decision making, is an area that is still to a very large degree unexplored, probably where we will see it emerging the most, will be in DeFi space because a lot of the decisions are relatively simple.

**Daniel Ospina:**

**[53:38]** At least you have clear criteria of what a good outcome is. We want the number to go up. If the treasury's worth more in a month from now than it's worth now, that's a good thing. OK, cool. That's clear. We can probably set a machine and algorithm to try to optimize for that without being too worried about what would happen. But then if I try to delegate to an algorithm to optimize for: “this community wants to be better”; and no one knows what that means and every person has a different idea of what that means, then, it's really, really hard to plug these algorithms. 

**Daniel Ospina:**

**[54:17]** And then we probably need a lot simpler algorithms that can be more of a support mechanism rather than doing the heavy lifting of decision making. Just because the question is so complex, and we can end up with a lot of sub-optimizations that has unintended consequences.

**Darcy Allen:**

**[54:35]** Just to add to that, it's super early and we've kind of got innovation and experimentation happening at multiple levels. So, there's this kind of classic distinction. Classic is very early in blockchain terms.  Between the governance of blockchains and the governance by blockchain. When we're talking about the governance of blockchains, we're talking about everything we've had in this conversation. How do we decide what to do with the Treasury or upgrade or whatever it is? That's the governance of blockchains, which is a hard problem. But at the same time, we've got governance by blockchains, so blockchains are powering up all these other technologies, like Daniel mentioned to enable automatic execution of the outputs of other algorithms, for instance.

**Darcy Allen:**

**[55:26]** Now, in my mind, sometimes we can flight the two things and it can make it really, complex; we're trying to solve multiple problems at the same time. I am super bullish on the opportunity for these algorithms as an input into governance decision making. I just worry sometimes, it's a little bit early and it's very experimental.

So, for instance, in treasury management, if you're talking about something like treasury diversification, it might be useful for you to have a committee making decisions about treasury diversification, but maybe they are informed by some kind of prediction market about how the treasury should be diversified, that it's an input into their decision but not necessarily throwing it all over to that straightaway.

**Darcy Allen:**

**[56:20]** But, there’s super exciting stuff going on in this space. As Daniel has mentioned a few times throughout this podcast, there's just so much work going into tooling, and I am very excited to see where we are in six months or a year's time. Six months ago, if you were trying to spin up a DAO, you were kind of doing everything from scratch in a way. I feel like if you're spinning up a DAO in a year's time, it'll be obvious that you need to do this and this and this, and you use this tool for that, and you'll still stuff it up, but you'll have a much better idea of what all those parts that need to come together, including algorithms.

**Eugene Leventhal:**

**[57:04]** And unfortunately, our time together is coming to an end for the day, but I appreciate all of the different ideas brought up and especially this point of experimentation and how much change is happening. That feels like a really appropriate note to be ending on, given in general how fast things are move in any tech and startup space, but especially in crypto. What is a day in a normal space and moves in a very different time here with just the amount of innovations in pockets of activity and innovation?

**Eugene Leventhal:**

**[57:34]** I know I’m really excited to likewise learn from all of these different projects and figure out how to best share and converse about them. But I just wanted to give everyone a chance to sort of plug any final thoughts or things that you’re just most kind of keen on and keeping an eye on as we kind of wrap this year and head into the new year.

**Darcy Allen:**

**[57:55]** I think you’re exactly right to focus on experimentation, and I think when we’re talking about treasuries and we’re talking about treasury attacks and all of these problems, we can get a little bit too focused on all of the threats to a treasury and not focus on the long term. How can we experiment with some tools and some things will go wrong, so that we can figure out how to best do this? And I think, as I mentioned, that happens in a polycentric way. And that has to be built in from an early stage. This idea that we are developing this DAO or this treasury with the idea that part of our mission is experimenting with our own governance structures because I think it’s harder to try and put that in after the fact. But I’ve really enjoyed this conversation and it’s super exciting to hear all the work that Daniel is doing as well now.

**Daniel Ospina:**

**[58:52]** Likewise. Very important points. In my language, I frame it as, they think about the DAO as a platform and like a basic platform where things are built on top and emerge on top, and we're really in the era of these platforms: the blockchain is a platform, the DAO is a platform built on top of the blockchain. And then we have other platforms and other applications built on top, and the teams themselves are platforms and so on and really embracing this mindset. Perhaps one single thing that I feel we didn't touch upon, that I would like to just put into the conversation even at the 11th hour: the importance of the individual mindset and kind of personal development as we go through this. 

**Daniel Ospina:**

**[59:37]** I think one of the most challenging things around being able to manage a treasury effectively and more generally DAOs and blockchains is the fact that decentralization means that we don't have a lot of control and something things don't go the way we initially intended, and we need to have a really strong grounding or self-like psychologically to feel, this is okay, it's an experiment. Let it happen and let other people chip into the conversation. Let the answer be a little bit more ambiguous than the perfect clear vision that I had at the beginning. 

**Daniel Ospina:**

**[1:00:17]** And I've been a victim of this, especially when I've recently been under a lot of pressure to deliver things. It's really easy to forget that no, wait, my idea is not the final one. We're in this together. And if we can do that and we can try to keep that grounding and be kind to each other, it's a lot easier to experiment and a lot easier to not obsess over the one failure compared to the 9 right that you got and rather move to the next cycle of experimentation, and invite people to participate when we can come from that place.

**Kelsey Nabben:**

**[1:00:50]** Yeah, thank you so much, Darcy and Daniel, it's been a really good learning experience, just conversing with you. I think some of the points that surfaced for me was really that point about polycentricity, and I'd love to see more examples of that being applied and kind of learning from those experiments. And Daniel, you mentioned a number of times about human readable systems. So, whether that's the contracts or the constitutions to keep them human readable. And I think that in the context of governance of and by algorithms is fascinating and a whole other episode. But thank you to SCRF for the opportunity to be here.

**Eugene Leventhal:**

**[1:01:29]** Yeah, thank you Kelsey, thank you Daniel, thank you Darcy. And we really appreciate everyone taking the time. Daniel, you especially ending with the personal development psychology of decentralization, could not have ended on a stronger tease for me conversationally. But we'll have to save that for another time, and we'll have to do a whole miniseries on the psychology of how to decentralize in the first place. But yeah, again, I do just want to thank everyone for taking their time to tune in to the interview and tremendously appreciative of our guests, Daniel, Darcy and Kelsey, for all taking the time to join us. This episode was part of our mini-series on building a treasury and funding public goods that we're producing in conjunction with RMIT. So please feel free to reach out to us on Twitter, over on smartcontractresearch.org if you want to be part of the conversation. Thanks again and be well, everyone. 

**Learn More About SCRF**

SCRF is an interactive forum supported by an active international community. SCRF’s members work together to advance actionable blockchain research. [Learn](https://github.com/smartcontractresearchforum/docs) more about SCRF, and discover ways to [get involved](https://github.com/smartcontractresearchforum/docs/blob/main/en/content_connecting_with_scrf.md)
