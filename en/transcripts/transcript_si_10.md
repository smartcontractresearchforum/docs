**The [Smart Contract Research Forum](https://www.smartcontractresearch.org/) (SCRF) has created a transcript of the most recent episode of the SCRF Interviews Podcast. For more information about the podcast, please click [here](https://www.smartcontractresearch.org/search?q=scrf%20interviews).** The first of two episodes dedicated to DAOstar One. At issue: Decentralized Autonomous Organizations (DAOs) lack a common technical standard that would make it easier for developers to create tooling for DAOs, and give DAOs the same level of legibility and interoperability that other web3 entities like NFTs currently enjoy. Featuring a discussion between Metagov Executive Director Joshua Tan and Isaac Patka, Co-creator of Logos DAO and contributor to Moloch Mystics. Moderated by SCRF’s Head of Operations, Eugene Leventhal.

**Eugene Leventhal:**

**[00:05]** Hello and welcome to the SCRF Interviews podcast in this mini series with DAOstar One, we're going to be exploring their DAO Start Standards Project and the intended impact in the industry resulting from it. We're glad to be joined in this first episode with Joshua Tan, who's the executive director of Metagov and Isaac Patka from Moloch Mystics. And I'll pass it off to you both for some intros. 

**Joshua Tan:**

**[00:28]** Sure. Thanks for having me here Eugene. I'm Josh. I'm the Executive Director of Metagov and a mathematician and computer scientist at Oxford and Stanford. Metagov itself is a nonprofit that does research in the space building standards and infrastructure for digital governance as well. Issac, would you go ahead.

**Issac Patka:**

**[00:45]** Sure, I’m Issac Patka. My primary thing that I work on is called Logos DAO, we have a DAO that basically connects people to DAOs and DAOs to other DAOs, and through that, I contribute to a number of DAO ecosystems with my team. So I work with MolochDAO, the Moloch Mystics ecosystem and the DAOhaus ecosystem and a lot of the DAOs  in the MetaCartel, RaidGuild, a lot of stuff throughout that whole ecosystem. I met Josh actually through two through two parallel channels that converge: one was this artist community that I was helping out and then also through a conference that MetaCartel was hosting called MCON and I'm just excited to get started.

**Eugene Leventhal:**

**[01:32]** So I think it would be interesting to start the conversation and we'll come back to this towards the end as well. But to start the conversation, what exactly is DAOstar One? And then we'll kind of take a step back to where it came from and really why does it exist? And then kind of dig into it a little deeper.  It would be great to kind of get a sense at a high level of how do you two position what DAOstar One is in general. 

**Joshua Tan:**

**[01:53]** So DAOstar One, most basically, is kind of a roundtable of different organizations, key organizations in the DAO ecosystem. So it ranges from, frameworks like Gnosis, Aragon, Colony, Syndicate to lots of DAO tooling developers like Tally, Abridged, Boardroom and so on, to aggregators like Massari and Ditto, as well as like major foundations like the Uni Foundation, Interchain . 

 **Joshua Tan:**

**[02:28]** So really a large panoply of different organizations, and of course, like large DAOs like Compound. The idea of the roundtable is to sort of like bring together a whole collection of different people, especially as key players for us, like building DAOs and sort of thinking about how do I implement these things at a technical level, in order to build technical standards? And the reason it exists is because also, in short, we wanted to build these standards and this roundtable; this group of people kind of just organically grew up around that standards process.

**Eugene Leventhal:**

**[03:04]** That's great. And Isaac, is that how you generally position it as well, or do you kind of give it a different flavor when you do your pitches explaining what DAOstar One is?

**Issac Patka:**

**[03:13]** Very aligned with Josh there. For me, DAOstar One is just an opportunity to improve legibility and access across DAOs and lead to further composability and tooling. The early problems that we're solving are essential to not just make DAOs easier to understand but also unlock many more opportunities for composable organizations and composable governance in the future. So it's catching this early, so that when as DAOs start propagating throughout companies and ecosystems and co-ops and neighborhoods and online and offline communities, that there is like a shared understanding of what we're actually what we're actually building.

**Eugene Leventhal:**

**[03:59]** Great. Thank you both.I guess to  get us to the point of “how did we get here” and “where did this come from” and “why is now the right time”,  it'd be interesting to hear a little bit about how DAOstar One came together in the first place. So Josh, do you mind mentioning kind of what were some of the genesis conversations or interactions that actually led to this?

**Joshua Tan:**

**[04:20]** So essentially it happened at MCON last year. So I think October 2021…September? And a group of us were kind of hanging out, having a couple of beers in the venue. So it was people from Aragon, Gnosis, Abridged, Tally, I think Spencer Graham was there, Ivan Fartunov, I don't think Key was there but maybe Orin was there James Young and essentially we were just talking: “Hey doesn't like a DAO standard already exists, like surely a must?” and then we realized - wait no actually it doesn't exist actually nobody agrees on what DAOs are. 

**Joshua Tan:**

**[05:08 ]** You bring ten experts into a single room it's like ten different definitions of what a DAO is and there were all these people building different projects, building different frameworks, different tooling with different expectations of what DAOs were,  and this, I think like somebody from Syndicate captured it really well, which is,they just said: “hey, we're not really confident building on any of these stacks because we're not really sure like, what the hell is going on. I don't think we have clear expectations and we're not sure, like any of this stuff is going to be around, even like one to two years from now, much as like ten years.”

**Joshua Tan:**

**[05:43]** So, there was clearly a need for a standard. We just decided that given that this doesn't already exist, we need to build one and we just said, “let's start building it”, and we started to set up a meeting, brought a bunch of people. We had our first kind of like roundtable meeting a couple of weeks right after MCON, virtually, and we decided, oh ETHDenver is about four months away, **]** that seems like a pretty good target, and we started driving toward getting a standard ready by then. I will definitely say that I can't believe it actually only took us four months in some sense, but that was, I think, bringing in exactly the right people, the people who know exactly what DAOs are have been building with them since day one. I think it was just a really awesome set of conversations and I think Isaac can speak more to that as well.

**Issac Patka:**

**[06:35]** I actually completely missed all of this happening at MCON. I had no idea that this conversation went down and that this all started there. I was there. I was probably at the picnic table about 100 yards away, but was completely ignorant to this whole thing. It was not until I think like a few weeks after MCON when I was on a call with the Data Art Community, and Josh popped in because Metagov was helping them design their DAO, community standards and stuff, and I mentioned this. Metagov inter-DAO standard thing, and I said, “wait, how did I miss this?” So I DM’d him quickly, got added to the Telegram, joined, and was just kind of thrilled to see the collaboration that was already starting to take off.

**Eugene Leventhal:**

**[07:13]** That's great. And just making sure for the initial kind of group of folks contributing to this and thinking about; is this all revolving around the Ethereum ecosystem broadly or is there a kind of wider collaboration of DAOs across ecosystems at this point?

**Issac Patka:**

**[07:27]** It's actually broader than that. Right now a lot of DAOs are in the Ethereum space, but I actually do a lot of outreach to DAOs on other chains as well. So specifically, like I know some art communities and Tezos that are starting to build DAOs, and the tooling is not quite as mature, but like I'm going into their Discord,reaching out, saying, “hey, here's, here's this thing that we could be doing together.” We know that like Josh working with some folks from other ecosystems as well. So definitely cross-chain is just the concentration of devs and liquidities on Ethereum, but other, definitely not Ethereum exclusive.

**Joshua Tan:**

**[08:01]** It was always intended to be multi-chain from the beginning, but we made a commitment sort of like early on to say, it's already a big thing to sort of say we're going to put together a EIP in time, within like four months. So we decided just because of that to really focus on the Ethereum ecosystem. But right now we are convened a group of people, including folks from like Cosmos Tezos, trying to bring on somebody I think we are close to bring on somebody from Polkadot to basically, and of course Near, to figure out what is the multichain standard: how can we extend existing Ethereum standard, EIP, into a kind of like a chain-agnostic improvement proposal. And that's currently something we're working on, and maybe hopefully you'll see something in about a month or two.

**Eugene Leventhal:**

**[08:51]** Ok, so hopefully and I'm assuming there's realistically going to be some delay between this conversation and release, so hopefully in the May-ish timeline, we will see some kind of update on that side?

**Joshua Tan:**

**[09:01]** Yeah, possibly sooner.

**Eugene Leventhal:**

**[09:03]** Cool. Exciting. I'm interested in kind of digging into a little bit around the question of why is interoperability so important, in general, when it comes to DAOs and smart contracts? What do you see as being limited without this, or what is not possible without these kinds of standards in place?

**Issac Patka:**

**[09:24]** I think that backing up slightly even further, when we talk about like what we're trying to accomplish with it with a DAO standard and interoperability, it's  more about legibility to start, and the reason why that's important is: right now what's not possible in a DAO ecosystem is to just quickly be able to peer into another DAO and get a quick understanding of what's going on. What's the state like? Who are the members of that DAO? What does that DAO even do? There's a random transaction on Etherscan; was that a person? Was that a DAO? Was that somebody interacting with a DAO? Ok, I heard about a DAO that decided to do something; how do I find that?

**Issac Patka:**

**[10:08]** So, this whole concept of where DAOs are, who is a member of that DAO, what that DAO manages, what that DAO is doing is very illegible and spread across many, many platforms. Often, when you try to learn about a DAO, it's like doing forensic analysis. You maybe start with a member on Twitter that  is in that DAO, Ok, did they retweet something that was from oh, Ok, there's the DAO Twitter, Ok they linked to a Discord, that Discord invite is dead. Ok, what what assets does this DAO hold? Do they have a website where they feature that or is it impossible to find? I'm interested in this DAO, can I join in? Oh, no, I have to DM someone and hope . . .  All of this is is kind of this state of DAOs.

**Issac Patka:**

**[10:51]** So it's impossible to aggregate data. It's impossible to just kind of get snapshots on what other DAOs are doing. And what that leads to is so much redundant work where you'll be doing something for a few weeks and think like this is going to be super helpful, and then often the next day you find somebody else that just spent the last two weeks coming to the same conclusion that you did.  To me, there's a whole ton of inefficiencies in the DAOs space due to this lack of legibility at the start.

**Joshua Tan:**

**[11:22]** Maybe we should define the terms a little bit. Interoperability - we often think of as like having one tool being able to communicate with another tool; technical interoperability where I have two services that are getting being able to communicate, having integration between Discord and let's say, I don't know, like Snapchat or something or like a lot of what Collab Land does: connecting to distinct services and getting them to communicate with another. 

**Joshua Tan:**

**[11:52]** When you have like interoperability, as a sort of basic assumption, you have this more, let's say, permissionless system where you can build things and expect them to work, you can plug and play different modules; and allows this sort of extensibility built in extensibility into the ecosystem. So it's really useful from a technical perspective for if you're like a DAO tooling developer. Now, in order to sort of support that, you often need to define, these like common like data schemas. And one thing that we do is we define a set of like very basic data models and schemas for these, at least, off chain kinds of data, and they're already proving useful for various DAO use cases. So they're effectively being used to support interoperability between different tools because these tools for the software these contracts share common assumptions about what data is being produced and the meaning of that data.

**Joshua Tan:**

**[12:52]** But the focus on legibility is to point out that, if we want to extend those use cases, extend these data models, support more interoperability and more use more DAO tooling sort of connections, we need to, sort of, enhance legibility of these organizations. So Zargham, for example, who is one of the co-authors of the standard, likes to emphasize that you need to do the reporting first. You need to emphasize this legibility first before you can really tackle all those additional use cases and really sort of, grab onto sort of a, what's the right word, benefit from the fruits of interoperability.

**Issac Patka:**

**[13:32]** The important aspect about this composability, and legibility, is that allowing people to do stuff with this that we don't that we can't even anticipate. A lot of people have this vision of this multi DAO future where DAOs are members of other DAOs and proposals are passed from DAO one to DAO two and that is a nightmare to manage unless we can at least all agree on how to describe data. And example that I think might help visualize in the Web3 space: If you go to Etherscan and you click on a contract, Etherscan knows that that's an NFT contract. It'll say ERC-721 or ERC-1155. There's even this rich explorer tabs where you can look at token transfers and you can see - even if it was masked within like a complex transaction on OpenSea or Rariable or somewhere, you can kind of see the flow of tokens and see like a pie chart of the top holders.

**Issac Patka:**

**[14:29]** All of that rich data is because we've all agreed on how to describe an NFT and ownership of an NFT. In the non-Web3 space and like the Web2 space, if you're on Google and you look for your local restaurant and when you look up a restaurant, Google knows that that's a restaurant and it's like, “OK, would you like to make a reservation here?”

**Issac Patka:**

**[14:49]** Here's our hours, here's how you get there, what's the general vibe? And all of that is also possible due to data standards. It's because we've agreed on how to define “this as a restaurant”, “this is a movie”, “this is a book.” And that's why we see rich data wherever we go on the Web. So, that type of rich data is; imagine attaching that to a DAO, and now whenever you see something related to a DAO’s transaction, you can see this rich data about “this is actually an organization that's deciding to add liquidity to a pool on balancer”, or “this is an organization that decided to send money to a coordinated epoch to distribute tokens to their members.” Like all of that rich stuff will become possible and people will be able to just leverage that for use cases that we haven't even imagined yet.

**Eugene Leventhal:**

**[15:38]** And so on that note, I want to kind of double-click into the whole idea of what is the kind of rich data that we're talking about here? And I know you alluded to sort of where it's coming from, where it's going, who are some of the actors? But what's sort of the data set that you would hope would be captured with something like this?

**Joshua Tan:**

**[15:54]** So, the actual data that's being captured is actually extremely simple. If you read the EIP, EIP-4824 to read the actual standard, or just go to DAOstar.org and you can click to the standard, it's online. You'll see like the scheme itself is extremely basic because, in some sense, we didn't want to over define things and sort of introduce overly rigid standards that don't match the actual use cases in DAOs.

**Joshua Tan:**

**[16:22]** And we also wanted to design something that's fundamentally extensible. So we just like build the basic things that we think “this is like DAO primitives” and then; let me backup, maybe jump into what the actual thing is. So basically, the standard imagines DAOs as really being defined by two extremely basic things. A DAO has behavior, which is just smart contract behavior, let's say. So that's inherited from the fact that it's a smart contract and a DAO has members. So it has behavior and members. And that is fundamentally, these are two primitive things about a DAO; and then sort of built on top of that, we assume that there is some way for the members of a DAO to meaningfully affect the behavior of the contract.

**Joshua Tan:**

**[17:12]** And that's how we define proposals as one mechanism, one very common mechanism for essentially membership to affect or influence the behavior of the contract. And this fundamentally is how philosophically the DAO is sort of the standard defines a DAO or looks at it. If you follow that, then it's actually very basic. So the EIP defines a set of members, so you can define a set of members of a DAO; and you can define the proposals that the DAO emits and then there's something called “an activity log” in which you can define certain relationships between members and proposals. So for example, like voting on a proposal, submitting a proposal, or executing something like that.

**Eugene Leventhal:**

**[18:01]** But also just like to take a quick detour into what is sort of the state of DAO tooling right now as it pertains to this and what is kind of the landscape and are there any things that do interact together or is it only within kind of stacks that are developed? So I'm sure all the Aragon tools can talk to each other on the data level, but is that sort of the extent of DAO tooling at the moment?

**Issac Patka:**

**[18:24]** One of my favorite bits of the DAO ecosystem that's being worked on is like the Zodiac Guild. So this is a group that started through through Gnosis, kind of attached to Gnosis safe ecosystem. And the purpose of Zodiac is to allow any governance framework or any rules to plug into a safe, which traditionally people think of as just a multisig, not just but like as a multisig with owners and an ability to execute. The Zodiac interface allows you to plug any governance framework that you want into that wallet without having to move any assets, without having to change anything.

**Issac Patka:**

**[19:05]** And so it's very useful if you're starting out a DAO and you want to deposit some funds and you don't want to have to like get locked into a framework. If you just put it into a safe you can upgrade governance over time. And a great example of this is the integration between DAOhaus and Gnosis through this interface. At DAOhouse, we had heard about this Zodiac interface being under development, we are working on a new version of a contract called a Minion which listens to a DAO and executes certain smart contract calls based on the actions of the DAO, and we were actually pretty close to releasing it when Decon from DAOhouse added me to a group chat with Oren from Gnosis and said, “Hey, Gnosis is going to come out, is going to announce this thing called Zodiac soon.

**Issac Patka:**

**[19:52]** I wonder if this would be useful for our minions.” And we looked at it and we thought, wow, this immediately allows us to rip out a bunch of code that we thought we had to write. And within about, I think we had like a proof of concept in a day and like a production version in a couple of weeks, we were able to prove that a DAO built on one framework could control a tool built by a completely separate group with completely separate rules without really any overlap between them. And tons of people are now building like modules through this Zodiac interface. I think it's a really good example of composability that's happening already.

**Eugene Leventhal:**

**[20:29]** That's great. And I guess are, from both of your perspectives, what are the things that you hope this kind of standard would be able to unlock, assuming of course, people readily use it? Because just the standard that is not adhered to is its own thing, but assuming there's buy-in and folks start doing this, like, what would you want to see in the first kind of months after wide adoption in the industry?

**Joshua Tan:**

**[20:49]** One of the first things we want to do, and we're already sort of  building supports and have gotten tentative agreement from folks like DeepDAO reaching out to [Unintelligible] and Etherscan, is to enable this kind of like DAO discovery and legibility. To have these DAOs, and to allow DAOs to publish the data and make it easily discoverable via these kinds of  aggregators and platforms.

**Joshua Tan:**

**[21:12]** So that's one of the very first things that we're doing. One of the use cases that we're currently actually right now working on, and it's quite exciting, I would say, is some use cases around DAO reputation or, identity systems within DAOs. So this is a work with part of a developing working group coming in that's happening in DAOstar One and extending the current EIP of folks like, Sismo, Spruce, DisCO, The Protocol, and other folks, Deep Skills. Working together to kind of find like how do we extend the basic database, the basic data model of members and activities to support these like verifiable credentials or like Web3 CVs; the ability to resubmit, prove that you are a member of a DAO, in good standing or you were a member of the DAO in good standing, and offer this to other DAOs. So you can say, “oh, now I can feel more comfortable hiring this person” various basic use cases that like directly extend the data model we put out.

**Joshua Tan:**

**[22:24]** We just need a little bit further agreement on it like how exactly to expose these kinds of credentials when DAOs publish that data and where things get stored and issues around privacy. Essentially questions that we actually discussed a lot in the original our working group that built the first standard, I realized was like too big a chunk to bite off in the first initial four months.

**Issac Patka:**

**[22:47]** I think that that would when we talk about things that people would actually use as far as a standard like that, to me has like instant, instant utility because when I am on Discord in my max 100 servers and I get a random DM from one of them, one of the first things I filter to see am I even going if I if the first thing I look at is like mutual servers.

**Issac Patka:**

**[23:10]** If it's one, I think spam, if it's nine I think, oh, real person. And then I click and see like, OK, which, which DAOs do I share? Like having that just gut check reputation reaction is something that is really important for when you're assessing whether you're going to interact with a certain address or,  anything like that. So I think that'd be super useful.

**Issac Patka:**

**[23:31]** Also use case that I would hope to see something that would show that we were successful is if I whether it's DeepDAO or Etherscan or something, if I can go to a DAO address and the DAO gets automatically tagged as, oh, this is an X type of DAOs Treasury, I would think that's that's already like such a ten X thing that helps me when I'm trying to just decipher what's going on.

**Issac Patka:**

**[23:55]** And one of the things that that I'm building with I mentioned like this LogosDAO is you can kind of think of it almost like an exchange for for DAOs, but like within a curated ecosystem and just making it so that at least within a small curated corner of the space, it's easy to know how I get into this DAO, what's going on with activity, like what do I need to keep an eye on because I fall behind all the time on like I have to sign this multisig transaction and I have to vote on this thing and I need some context for this thing before I feel comfortable voting on it. So at least starting with a small curated section of DAOs, I'm planning on at least using all of this rich data to help build that exchange functionality.

**Eugene Leventhal:**

**[24:41]** That's really interesting. And that also just makes me think of I mean, some of these elements I think are clear to understand of how they live in the data but when it comes to elements of, my presence in 10 DAOs versus the quality of my contribution in 10 DAOs are also very different. And, things like onboarding and making it easier to actually delve into a system and know what's actually going on there or even the quality of a DAO of, oh, they have 10,000 members, but is it just 10,000 people aping into something with no actual intention of building a community?

**Eugene Leventhal:**

**[25:13]** And I guess how do both of you think of  some of the elements that start being much more qualitative in nature and how you bring it back down to kind of data and metrics when it comes to standards like this.

**Joshua Tan:**

**[25:24]** At least from my perspective, it's a really hard question and it's really visible in the conversations that I have as part of the DAOstar One one actually. So as you can imagine, the standards body has a lot of let's say DAO tooling companies or also DAO tooling dumps. Right. But these people who are interested in building tooling and technical infrastructure support, like better DAO governance, better DAO operations and variety of different things.

**Joshua Tan:**

**[25:53]** Right. Or like DAO frameworks for creating like the literal DAOs themselves and these folks care a lot about, these standards because they're like the things like these data models they have to work with every single day. Right. And it's really important they get them right and ideally, like minimize the amount of change they have to do and facilitate  lots of things like interoperability and extensibility.

**Joshua Tan:**

**[26:16]** But like when I talked to the DAOs themselves, they care about these particular use cases right around, oh, how can I manage these contributors? How do I sort of foster engagement? And it's not like a question that a standard on its own can directly address. The standard is the way I think about it. It's built to support all this additional tooling that can then more easily tackle all these sort of end use cases that we care about, like, things like legibility or, contributions or management engagement.

**Eugene Leventhal:**

**[26:53]** And that also makes me wonder if at all in terms of various DAO tooling companies have any actually given any kind of pushback? Because I'm just, putting my Web2 lens on things, back on. Right. I can see how someone says, oh, well, actually complying with this kind of standard, while it gives us more interoperability with the ecosystem can make us somehow lose our proprietary advantage.

**Eugene Leventhal:**

**[27:15]** And I realize this is very much against the ethos of open source development and everything. But so I'm just wondering, I don't know, has that been a thing? And I'm sure you all have talked to hundreds of DAOs, hundreds of DAO contributors across hundreds of DAOs. Has that actually been a point of pushback or is everyone kind of on the open source bandwagon and into it?

**Joshua Tan:**

**[27:33]** Amazingly, no. There's been exactly zero pushback and everybody in this ecosystem is super. It's like they say, oh, what a DAO standard. Like exactly what we need this, let's do this. We are 100% in and it's like it's actually kind of amazing the amount of immediate, I guess, traction and enthusiasm that we see because I think people here are very much like,  if you're building in crypto, like there's an expectation that you are going to be like relatively open source and throw open with your data because I think that's just really the ethos of this community. ** **And I think it's wonderful and that we're focused on building interoperable protocols and supporting this kind of like it's say, ecosystem public goods.

**Issac Patka:**

**[28:17]** Also something that Spencer said on our first call, Spencer Graham from the DAOhaus was, correct me if I get the quote wrong Josh, but let's challenge each other not to build empires. To me, my interpretation is like, this is an ecosystem where people believe in positive sum collaborations. And when what we're working on together is going to be so much greater than what we can do individually, as the DAO standard matures and there like very focused platforms that spin up to kind of Web 3-ify, different community chats or groups and stuff.

**Issac Patka:**

**[28:53]** I bet we will see who self-select into this type of standards community versus who is like, OK, well, we can just add crypto to a message group, charge a subscription fee for it and see if that becomes a company. I'm sure those exist, but they're probably just not self-selecting into the kinds of conversations that we're having. And hopefully we can build better products together in this more open ecosystem.

**Eugene Leventhal:**

**[29:24]** It's great hearing that's the case so far in driving the standard forward. And I still am always fascinated by looking at DAOs and kind of exploring what's happening in communities from the perspective of how does ego management work in these environments. And, like some of these things are a little counter to at least growing up in the States and being taught to think certain ways.

**Eugene Leventhal:**

**[29:45]** And so I wonder, as you're going through and planning the actual technical infrastructure, you're building the community, getting all the relevant stakeholders in there, is there an element of just culture change that either, we either need to reinforce already some of what's happening or just an actual pivot around culture and thinking to make everyone be excited about these kinds of changes.

**Issac Patka:**

**[30:07]** There is some unlearning that has to happen when people move from like the Web2 space into the Web3 space. And for me, it was was actually nice. Like when II broke into like certain more collaborative aspects of the Web3 space, I got to think like, Ok, my natural tendency towards collaboration and openness is not a business weakness as it might feel like it is when you're trying to build just like a normal startup. I think that for people that have had to operate in that ecosystem, they do have to  think, OK, not building mode stickiness for like I'm not like you think in different types of terms. You think about extensibility and compose ability and value creation. So for me, it was nice because I was like thinking that I would have to go down the unlearning path of unlearning collaboration and go towards being more competitive. But I've enjoyed the fact that I've been able to just strengthen my collaborative side.

**Joshua Tan:**

**[31:04]** And I would just add, I absolutely agree. And maybe what I've noticed is that in some ways if you compare this like to, let's say, previous eras in Internet history, there's much more because like, the open source sort of ethos is so much more developed I think because crypto, what is it somebody said like crypto is like terribly explained because it's very technical in lots of ways.

**Joshua Tan:**

**[31:30]** And the people were trying to explain it like choose technical explanations. I think that sort of more engineering ethos has really benefited and carried over into the decision that these organizations actually make in terms of collaboration instead of building legal moats or  business moats around certain products and really focus on achieving technical goals and producing really cool technology. I think it's still very much we're still in that phase where I think all this cool tech is being built and we're just exploring this ecosystem and everybody  feels much more free.

**Eugene Leventhal:**

**[32:06]** And it's so interesting to think about that kind of unlearning side  because part of what I was hearing and what you were just saying, Josh, is the fact that I feel like a lot of the people who self-selected into building this industry were the kind of people who are already deeply bought into open source and had a certain personal ethos.

**Eugene Leventhal:**

**[32:22]** And I mean, it's not fair to brush to paint everyone with the same color brush, but I feel like it had a higher proportion than other, new tech startup areas. And the question of unlearning is a really interesting one because I know when I first got into it, there was very much like the mindset shift that I had to continuously remind myself of. And  that it's like, no, it's this thing that I'm naturally into. But was dis-encouraged in the corporate environment. But I wonder,  have you seen or is there something that you would like to see in terms of more structured unlearning when coming into this space? Because I see a lot of, like onboarding Web2 people into Web3.

**Eugene Leventhal:**

**[32:58]** It's like, oh, well, let's get them explainers on blockchain and let's get them a DAO Wiki and let's get them all these things to explain how amazing the things that we're doing are. And I haven't heard as much, but let's focus on how much you like working with other people and like, let's start from that, truly human collaborative perspective.

**Issac Patka:**

**[33:15]** That would be really interesting, there's not nearly enough resources on that side of blockchain, which is like how to re-educate yourself for the Web3 space and like, I think that's something like that targeted towards people that have gone through Web2 startup accelerators and like maybe somebody that went through those didn't really go through those.

**Issac Patka:**

**[33:39]** But like here's what you learned. Here's how it's different. Like that would be a very interesting content series because I deal with a lot of folks that have had long careers in the Web2 space. And I just do that one by one every time I have a phone call with them. But perhaps that would be a nice content series.

**Joshua Tan:**

**[33:56]** I should also point out that these kinds of collaborations and maybe this is something to put my research academic hat on, arrive or are possible because of certain institutions, right? There are technical products that allow, let's say, relatively decentralized collaboration that facilitate this kind of like one to one or, many to many sort of peer production.

**Joshua Tan:**

**[34:23]** And there are institutions, DAOstar One among them, to facilitate partnerships between different organizations. Sort of conglomerations of group of people that facilitate connections, communication, and ultimately collaboration instead of competition. So I think many maybe, we're saying of this we should pay respect to previous generations of people, of the Internet, of even Web 2 that are produced infrastructure that we're using things like,  Git and GitHub right that we use to collaborate and that, have set certain defaults for us in terms of how we collaborate and how we work together.

**Joshua Tan:**

**[35:07]** And those things are amazing. And we're just now building more institutions. And really, I think diving into that and committing to that ethos and taking it, I think, to its next progression. I think that's one of the truly exciting things about the space where we're so we're all trying to work together.

**Issac Patka:**

**[35:26]** That’s a great analog. Like I think about when I have the moment where I first decide I'm going to try, I'm going to test out this DAO, see if I can collaborate, see if they're a welcoming bunch. It's kind of the same feeling I get when I find an open source tool on GitHub that I'm using and maybe found a bug in.

**Issac Patka:**

**[35:43]** And I file an issue. And then I think, well, maybe I'll just file a pull request and fix it myself, and then you file it and the dev responds, Thank you so much for contributing to this. And you fix it and then your thing gets merged. And now you're a forever in the Git history of this tool that you like. It's a very similar feeling. And you're right, that was built, that infrastructure has enabled everything else that we're doing. Like open source, collaborative repositories have made it so that we can get to this point.

**Eugene Leventhal:**

**[36:13]** It's interesting to think of what are, what are the right ways to both pay respect to the tools and people who got us here while simultaneously unlearning the societal and kind of corporate mentality that might have unintentionally creeped into some of those because also just thinking of previous iterations of startups and everything and the complaint of like the startup or founder journey of going from ideological purity to then investing and growth phase, and then it becomes a very different kind of game.

**Eugene Leventhal:**

**[36:38]** But recognizing that we're unfortunately getting to the tail end of the conversation, I wanted to make sure to give a chance to just talk about, for folks who actually want to be part of helping move these kinds of things forward and contribute to this what are the ways that people can actually get involved and collaborate with the DAOstar One community?

**Joshua Tan:**

**[36:56]** Absolutely. So we host open Community Call every two weeks. You can go [DAOstar.org](https://daostar.org/) I think there are currently Thursdays at around noon Eastern Time in the US and they're open to anybody hop on in. Tell us what you think about the standards that we're working on. Tell us what you think could be improved.

**Joshua Tan:**

**[37:19]** Tell us about your use case and how our center kind of sucks and doesn't address it. We would love to sort of get you to participate. And if you're an organization that's building tooling or just a DAO that is thinking about upgrading to the standard, please reach out to Isaac myself or just hop on like a website again and just like contact us. We really love to work with you to figure out how to make the standard worthwhile and workable for you.

**Eugene Leventhal:**

**[37:47]** And if I'm not mistaken, DAOstar is also in a phase right now where it's actually trying to fundraise to be able to build all these activities and do all the all the various time intensive efforts necessary to make this happen. Am I correct on that side?

**Issac Patka:**

**[38:01]** Yes. A lot of the member organizations are also contributing to funding for things like reference implementations and reviews and everything that helps the standard operating and propagate throughout the ecosystem. So it's actually quite important to us that anybody that contributes to this is bought in ideologically and is contributing to the groups and has some commitment to adopting the standard as it comes out.

**Issac Patka:**

**[38:30]** We're thinking about different ways to play with incentives for organizations to adopt this beyond intrinsic. So if you also want to play around with incentive models and how those standards get adopted, lots of room for experimentation there. And if you're a developer that wants to dive in and build reference implementations, there's funding for you to come in and help.

**Eugene Leventhal:**

**[38:51]** Awesome. And is there anything else that you both want to mention about the initiative or or just getting this kind of activity started that we didn't touch on in the conversation?

**Joshua Tan:**

**[39:00]** Maybe I'll mention one thing, we are going to be announcing something at DevConnect in Amsterdam, so that'll be late April. So if you're around, come by, we'll be having some events related to DAOstar One and the standard.

**Issac Patka:**

**[39:14]** We pop up in various different governance conversations and conferences all over all over the place. So if you see us, then I hope to see you in person at some point soon.

**Eugene Leventhal:**

**[39:25]** Absolutely. And slight shameless plug in a different direction. On the DevConnect week. There's also going to be a DeSci day in Amsterdam that week, which should be fun and provide a bunch of different opportunities for folks to talk about activities at the intersection of decentralization and science. But anyway, thank you both for joining us today. This is a great conversation and thank you to the listeners for joining in and listening to SCRF interviews.

**Eugene Leventhal:**

**[39:46]** If you want to learn more about DAOstar, please check out their site. [DAOstar.org](https://daostar.org/). This podcast was brought to you by the Smart Contract Research Forum, or SCRF. The SCRF Interview Team consists of myself, Eugene, Ivan, Rich, James, Lorretta and Tebogo. To learn more about SCRF, check out [smartcontractresearch.org](https://www.smartcontractresearch.org/) and we'll have a specific forum post up for this episode where you can interact and ask some questions there. If for whatever reason you're too shy to just get right involved in the DAOstar stuff. Thank you both again and have a great day.
