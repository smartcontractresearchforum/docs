# SCRF Central Bank Digital Currency (CBDC) and Blockchain Panel Transcript 

The[ Smart Contract Research Forum](https://www.smartcontractresearch.org/) (SCRF) created the CBDC and Blockchain Panel Transcript for those interested in DeFi to learn how CBDCs are evolving in relation to the blockchain.

## Overview

This is the transcript from the CBDC and Blockchain Panel that was organized by SCRF as part of the Smart Contract Summit in 2021. To read more about the panel, the panelists, and the topic, refer to the [forum post](https://www.smartcontractresearch.org/t/smart-contract-summit-2021-central-bank-digital-currency-cbdcs-blockchain-panel/623).

## Transcript

**Eugene Leventhal:**

Thank you for joining us today for a panel discussion. I am Eugene Leventhal, the Operations Lead here at the Smart Contract Research Forum, and we’re excited to be moderating a few panels as part of the Smart Contract Research Forum Stack. To get us started, I’ll just go around and ask our panelists to do some introductions. Andrew, do you mind kicking us off there?

**Andrew Miller:**

[00:31] Sure, thanks Eugene. Very happy to get started. I’m Andrew Miller. I’m an assistant professor in computer engineering at the University of Illinois. There, I lead the Decentralized Systems Lab and my research mainly focuses on cryptography, programming languages, blockchain design, a lot of smart contract programming - the technical side of cryptocurrencies.

I’ve been in the blockchain space for about nine years; I was in, I think, the first cohort of folks who did their Ph.D. dissertations focused on cryptocurrencies. All that is to say, I think I have a good grasp on the technical side of blockchains and maybe on the cryptocurrency ecosystem’s view of narratives and how finance works. But I’m very new to learning anything about mainstream finance or central banks or real-world banks work.

[1:21] I think I’m on this panel because I co-authored (with some other folks at the Initiative for Cryptocurrencies and Contracts) a paper on design choices for [Central Bank Digital Currencies]. I mostly have perspective on what kinds of programming interfaces CBDCs might have and what kinds of privacy issues and techniques that they would have. I’m interested in learning from some other perspectives, for example, on the kind of institutional and organizational, and policy issues of CBDCs.

[1:53] You’ve asked me to give an explanation of what a CBDC is… To me, from a developer’s perspective or the blockchain perspective, I think the definition has to be pretty loose. I would call something a CBDC, for example, if it were centrally operated and directed retail customers to a central bank or something that’s more hierarchical with member banks and commercial banks involved.

To me, what makes something a CBDC is if it incorporates any kind of blockchain technology, whether it’s cryptography to provide privacy or smart contract programming to provide extensibility. And what I expect is likely to emerge as the real promising pattern is the idea of a central bank providing an API [Application Program Interface] platform for programming, with some kinds of rules or regulations or constraints built-in at the platform level.

[2:48] But then a very high amount of flexibility for commercial banks and member banks to be able to customize their own applications through this programming interface, and then compete on the kind of functionality that they could offer. It’s really the CBDC as a platform kind of view. I’ll yield there.

**Eugene Leventhal:**

Thank you, Andrew. Ariel, do you mind going next?

**Ariel Zetlin-Jones:**

[3:11] Sure, thanks Eugene. My name is Ariel Zetlin-Jones, I’m an economist at the Tepper School of Business at Carnegie Mellon University. My research focuses on how information and technology shape financial markets and the implications of financial markets, and financial market regulation for the broader macroeconomy. Lately, I’ve been studying the role of blockchain and disrupting financial markets and thinking about what economics can shed light on for the blockchain and aspects of computer science.

For example, I’ve been thinking about how to harness economic incentives to improve consensus on distributed ledgers, or how to use economic incentives to improve, in theory, the design of stablecoins. With my training in macroeconomics and monetary economics, I’ve thought a lot about the role of government and private payment systems in the macroeconomy. And so the perspective I’ll try to add is kind of the interaction between what monetary policy and central bank digital currency may or may not achieve in changing our payment system.

[4:09] I have a very similar perspective to Andrew in terms of what a Central Bank Digital Currency may be. I think the critical distinction is whether we think a CBDC is only going to be accessible by financial institutions, or accessible to retail customers. And I think the most interesting aspects, as Andrew suggested, is that what’s new about CBDCs is offering access to a savings account at the central bank for retail customers and whether that’s an account-based system, or a token-based system is an interesting question.

[4:41] I think that’s the newest aspect of a central bank digital currency. And then the question is how will this impact our payment system? How will this impact the traditional banking system? And what does it imply for monetary policy? Those are, I think, all interesting questions to start thinking about.

**Eugene Leventhal:**

Great, thank you, Ariel. And Phillip, do you mind jumping in next?

**Philipp Sandner:**

[5:02] Thanks, yes. My name is Philipp Sandner, I’m working at the Frankfurt School of Finance and Management, which is a small university in Germany. Not everybody might know this university, as I said, it’s a small one. We have 400 business faculties over here in Germany, and the Frankfurt School belongs in the top 10 over there. So people over here know it, but it’s a tiny one, therefore, not everybody out there might know our university.

I myself have been into blockchain knowledge since 2013 when I discovered Bitcoin, which became a kind of hobby in the beginning. Five years ago, we set up the blockchain center at the Frankfurt School. And since then with our team of 10 people, we have been doing full-time blockchain crypto DLT [Distributed Ledger Technology], but we also moved away from enterprise solutions towards decentralized systems and cryptocurrencies. That’s where my heart lies nowadays with on-chain analytics and so on.

[5:56] One interesting topic we are currently investigating is what kind of tokens are out there. You have utility tokens, payment tokens, investment tokens, these tokens, that tokens and bringing some kind of structure to what is out there is one of the missions in our research. And historically, I’ve studied a mixture between business and computer science. And from a research perspective, I do a lot of work in the area of entrepreneurship and also venture capital, always with empirical data.

And now concerning CBDC, I think I would follow your explanation and your definition. Definitely, I would try to define CBDC as some kind of… let’s call it, digital modern ledger, where a central bank tries to reestablish the direct relationship to its customers. It can be mediated through financial intermediaries, such as banks or payment providers, but not necessarily.

[6:52] And Miller is absolutely right, CBDCs can be DLT based, but they do not have to be DLT based. They can have smart contracts, but they do not have to have smart contract functionality. And therefore there are good reasons why blockchain technology makes sense, but central banks around the world are also experimenting with non-blockchain CBDC’s.

[7:14] Therefore, I think my perspective is that CBDC is only one sort of digital money of the future, there will be other sorts of money, some of them will be fiat-based, some money will be not fiat-based. In Germany, for example, we discuss this a lot. How, for example, do we leverage blockchain and the Euro. In smart contracts, how do we leverage the Euro in smart contracts as soon as possible, because the ECB [European Central Bank] tried to build a CBDC, but the ECB is lagging quite strongly behind China. A CBDC produced by the European Central Bank might be with us by 2026 or 2028.

[8:00] And this move is strongly opposed by European industry, companies like Daimler, Bosch, Siemens are urgently demanding a digital currency. So there need to be other forms of digital Euro because the CBDC is a big project and apparently the ECB is not the fastest organization out there.

**Eugene Leventhal:**

Great, thank you for introducing yourselves. And we also have Richard Brown joining us, who is the co-founder of SCRF. Rich, do you want to give a quick intro too?

**Richard Brown:**

[8:32] Sure, I’ll make this super brief. I’m Richard Brown co-founder of SCRF, most recently head of community at MakerDAO. If I have any experiences relevant to this conversation, it is that we produced a stablecoin and there are some obvious similarities between that and some of the proposals for CBDCs, I’ll be co-moderating with Eugene, and as I’m a neophyte in the space I’m looking forward to the conversation, but I don’t think I’ll have much to add but am looking forward to it. Thank you, Eugene.

**Eugene Leventhal:**

[9:06] And so to get us started, I want to follow up on the kind of definitions that you all laid out and zoom in on that idea for a moment. Because I think trying to create a baseline of “what is a CBDC” in relation to “does it need to be using a DLT or smart contracts or some of these other blockchain technical components” or not is helpful. Philipp, you mentioned the idea of hybrid CBDCs when we were getting started.

[9:41] Philipp, do you mind mentioning what you mean by hybrid CBDCs, what those are, and then we’ll springboard into what we see as the minimum design requirements for something to be a CBDC versus another type of tool that central banks might be able to have at their disposal?

**Philipp Sandner:**

[9:58] Yeah, exactly. There are multiple design options out there for CBDCs. Typically, you call it direct CBDC, if we as citizens have direct access to the central bank. But this would require the central bank to really do IT, it also would require the central bank potentially to run an online app, like a smartphone app to give access to the Euro or the US dollar.

[10:23] I think central banks are not the right organizations to supply such IT. Therefore, the topic of hybrid CBDC’s popped up, this means that the central bank is applying the money originally, but it also relies on existing banks and payment providers to process these payments, to also onboard customers to do KYC [Know Your Customer] processes and AML [Anti-Money Laundering] checks. This way you have a multi-tier system with the central bank in the background, and some banks and payment processes in between.

[10:57] And the most important point here is that the central bank is supplying the money originally with inflation, without inflation, it doesn’t matter, but it’s supplying the money and the money can then be taken up by banks and be forwarded to us as citizens, but also to companies and so on. And most important on this point is that there are also payment processes, such as credit cards and banks who are then themselves supplying citizens, and who are also supplying companies like Bosch, Daimler, Siemens, all these companies, they also need cash for their payments.

[11:31] And here, I think it’s very important to note that a central bank is not necessarily always bridging the entire line from a central bank to its citizens, but that it supplies money, which can also then be used by other payment processors, who then themselves make money available to the capital markets, to the industry, to the upcoming economy of things and so on. And that’s why the topic of hybrid CBDCs could potentially make sense.

[12:02] And the last point I would like to make, in Germany we have this discussion going up of what we can do to supply companies with some kind of digital currency, with a digital Euro. And here, for example, banks are developing some payment adapters which are sitting in between the legacy payment systems and smart contract systems, and they are trying to reconcile a blockchain system and the balances there with the money in legacy payment infrastructures in the bank accounts. And these payment adapters are then trying to synchronize the legacy world with the modern blockchain-based payment infrastructures.

**Eugene Leventhal:**

Great. Ariel, did you want to jump in?

**Ariel Zetlin-Jones:**

[12:51] I do, I really appreciate Philipp’s perspective about this possibility of a hybrid system. And I think it’s important to recognize we sort of live in that system already, at least in most advanced economies, right? Where central banks provide physical currency that are used directly by retail customers, but they also provide reserves indirectly to the commercial banking system who then supply their own form of private money supported by those reserves to private customers.

I think what Philipp is describing is that the role of these banks may look very different when the central bank issues its own digital medium of exchange, that is in principle accessible by customers. That maybe their platform providers have some way to give a better IT experience, better access to central bank currency than just creating their own private money.

[13:36] And I think that tension is an interesting one, and I think the big challenge from a central banking perspective of thinking about creating a digital currency is exactly the fact that right now the intermediaries play two different roles. There are payment processors, but there are also the people who extend credit, the institutions responsible for extending credit.

[13:56] And so the big debate in the economics literature right now about CBDCs has really been focusing on disintermediation. The idea that if you give retail customers direct access to the central bank to store their savings, will they no longer save in the commercial banking system? I think that’s why in advanced economies you’re seeing a push for some kind of hybrid approach to make sure that we can leave resources in the banking sector to keep extending credit.

[14:20] Because I don’t think central banks are interested in using these deposit reserves to extend credit themselves. And so that’s why I think Philipp’s perspective is very interesting and useful one, the question is just, will the role of these intermediaries change if we create this new kind of digital media?

**Eugene Leventhal:**

Yeah, of course. And Andrew, did you want to jump in here as well?

**Andrew Miller:**

[14:41] Yeah, I liked the framing of your question as to “what would be a minimum viable CBDC,” “what’s the minimum amount of blockchain technology that could be added to it” and still call it on blockchain-based or a digital currency? I mean, one thing that I would mention is that, I think it’s unlikely that you could have a CBDC built on top of a public blockchain, for example, or built on top of proof of work anonymous consensus systems, for example.

It’s more plausible that it would be some sort of consortium consensus protocol or even something that doesn’t even resemble a consensus protocol and is essentially centrally operated and looks a lot like an ordinary database system. I could give some examples of potential technical crypto benefits that you might get even in a centrally administered database that I think still are very much kind of responsive to the things that are desirable about cryptocurrencies and blockchain.

[15:36] The example that I will give is the idea of auditability and transparency for records. To the extent that people are interested in being able to audit from a public viewpoint, otherwise opaque systems of how much money is being printed or how it’s going around. Some of the kind of technical toolkits in blockchains, like hash-based data structures and commitments, for example, could be used to essentially make a public account record of all of the main movements, or changes to parameters, or changes to interest rates, or other kinds of things that might change over time.

[16:21] And some of the technology that blockchains use today in the cryptocurrency world, like zero-knowledge proofs could be a really good fit for that as well. You might be able to provide a very good open transparency record, that’s essentially a proof that a certain policy has been abided by the central bank or by the member banks. You’d get some cryptographic proof that the rules that were set were followed to a T.

[16:47] And that’s something that’s new. I think right now, in an opaque central database system, all you can do is take the administrator’s word for it. Cryptocurrencies show that there are some alternative approaches that could be better than that. Even in the world where we are now, to say nothing of the programmability frameworks, like smart contracts or the distributed trust like consensus protocols. Even if nothing else, one could imagine CBDCs incorporate some of the cryptography components that blockchains use for better auditability.

**Eugene Leventhal:**

[17:20] I appreciate what was mentioned so far, especially in terms of many of the conversations from pure DeFi protocols or anyone that’s purely in the blockchain space is just disintermediating the existing financial system. But if a central bank deploys this technology, there’s the added tension of, well, how do we actually keep the stakeholders in the loop and as part of this new future and not dis-intermediate them away? That was just an interesting thread that was mentioned there, but Rich, did you want to jump in and mention something?

**Richard Brown:**

[17:50] Sure, there are some interesting things to unpack here. It’s the blockchain space, sort of, disintermediate and then the central banks issue CBDCs, and then they re-intermediate themselves. But the distinction that DLT is not a given, it’s more of the paradigm and the assumptions that come along with this new sort of blockchain world that we live in, that the banks are now competing against the private sector, which is offering programmability and a greater audit trails and perhaps more responsiveness to transactions.

[18:25] It’s the banks waking up to this new world that there are expectations that they will provide platforms. And so does that turn traditional banking into more of a Fintech model, where the banks or the settlement layers are the issue, the token mentors and normal banks that we’re familiar with become Fintech platforms? Is that the new world that we’re looking at?

**Eugene Leventhal:**

Phillip, I know you had your hand raised, if you want to respond to that one or a follow-up on a previous thread?

**Philipp Sandner:**

Well, I think that’s a very, very interesting thought. Like doing finance platform and basically providing access to money, could also be other monies, it doesn’t need to be one currency can also be foreign currencies and so on. Makes extremely much sense for a bank, and I think the governments around the world, they will always want to have organizations in place such as banks who are doing identification of customers, who are doing ML checks and so on.

**Philipp Sandner:**

And I think if you are seeing a world where governments are requiring this, somebody has to do it. And I think this is a task, which is basically as in the past, also loaded on to our existing financial intermediaries, even if potentially in the future, you’re taking the possibility of providing loans away from banks. But I would like to add one more point to what Andrew has said.

**Philipp Sandner:**

I think one of the very interesting point of blockchain technology, which very often is not really understood is, that you have one lecture and you have multiple assets on top of the lecture. You see this very nicely happening in the Ethereum world with defy, right? That in case we are talking about money and central banks of the past and the ECB and the fed and other central banks around, they are simply operating their silo.

**Philipp Sandner:**

And they don’t really care what’s happening with the Euro, or to the Euro, or the with the US dollar. They are simply supplying the Euro and the dollar, and that’s your silo, right? But if you’re doing transactions, security transactions in the capital market, in case you’re purchasing a product or a service from an industrial corporation, then you are giving money and you’re taking something.

**Philipp Sandner:**

There is a give and take taking place, and this give and take in the capital market is operated by clearinghouses, right? And once you have a blockchain system, which is token-based, and you can have the Euro to dollar securities and other forms of assets on top of one of the same platform, then you can get rid of clearinghouses. Because the clearinghouse function is then done and executed by smart contracts.

**Philipp Sandner:**

That’s exactly why DeFi works so extremely well, because you don’t have clearinghouses, informs of organizations doing this, but you simply have smart contracts. And this is an angle in my mind where blockchain technology for CBDCs really, really make sense, but central banks around the world have to accept that in the future not simply operate their silo of money, but they are deploying some kind of currency on one lecture, where potentially there could be other assets as well.

**Philipp Sandner:**

Because only if you have a multi-asset platform, then you can leverage smart contracts, settlement by smart contracts. And then you can get rid of clearinghouses with all the efficiencies and costs and time and insurances and risks and so on, which you then do not have any more ones clearinghouses are not needed anymore. I think that’s a very important point, which is very often not fully understood.

[18:55] Well, I think that’s a very, very interesting thought. Like doing a finance platform and basically providing access to money, could also be other monies, it doesn’t need to be one currency, it can also be foreign currencies, and so on. Makes sense for a bank, and I think the governments around the world will always want to have organizations in place such as banks who are doing identification of customers, who are doing AML checks, and so on.

And I think if you are seeing a world where governments are requiring this, somebody has to do it. And I think this is a task, which is basically as in the past, also loaded on to our existing financial intermediaries, even if potentially in the future, you’re taking the possibility of providing loans away from banks. But I would like to add one more point to what Andrew has said.

[19:54] I think one of the very interesting points of blockchain technology, which very often is not really understood, is that you have one ledger and you have multiple assets on top of the ledger. You see this very nicely happening in the Ethereum world with DeFi, right? But in case we are talking about money and central banks of the past and the ECB and the Fed and other central banks around, they are simply operating their silo.

[20:18] And they don’t really care what’s happening with the Euro, or to the Euro, or the with the US dollar. They are simply supplying the Euro and the dollar, and that’s your silo, right? But if you’re doing transactions, security transactions in the capital market, in case you’re purchasing a product or a service from an industrial corporation, then you are giving money and you’re taking something.

There is a give and take taking place, and this give and take in the capital market is operated by clearinghouses, right? And once you have a blockchain system, which is token-based, and you can have the Euro, the dollar securities, and other forms of assets on top of one of the same platforms, then you can get rid of clearinghouses. Because the clearinghouse function is then done and executed by smart contracts.

[21:05] That’s exactly why DeFi works so extremely well; because you don’t have clearinghouses, in forms of organizations doing this, you simply have smart contracts. And this is an angle in my mind where blockchain technology for CBDCs really, really make sense, but central banks around the world have to accept that in the future they may not simply operate their silo of money, but they are deploying some kind of currency on one ledger, where potentially there could be other assets as well.

[21:32] Because only if you have a multi-asset platform, then you can leverage smart contracts, settlement by smart contracts. And then you can get rid of clearinghouses with all the efficiencies and costs and time and insurances and risks and so on, which you then do not have any more ones. Clearinghouses are not needed anymore. I think that’s a very important point, which is very often not fully understood.

**Eugene Leventhal:**

[21:59] And that also generally makes me wonder about the importance of how much pre-planning and standardization needs to be done to enable interoperability on a global scale versus how much as with many crypto projects that will build first and figure out the details later on some of these things. But Ariel, I know you wanted to jump in.

**Ariel Zetlin-Jones:**

[22:18] Well, I just wanted to raise, that there are risks of interoperability across currencies. And making currencies very easily tradable on the exact same platform jointly with say goods or services, capital being traded creates risks for independent control of monetary policy. And so we could see resistance to this usage, as Philipp is describing, of a Central Bank Digital Currency, where you’re creating a single platform and there’s some academic research already showing this.

What do global digital currencies imply for the risk of independent monetary policy? I did want to follow up on one of Andrew’s points though about using the underlying technology features of blockchain in a CBDC, perhaps in a centralized ledger way. And what I thought was fascinating of Andrew’s perspective is that, a CBDC could be used as a way to gain transparency into monetary policy.

[23:09] The flip side perspective is the ability of a central bank to gain more transparency into the use of its money by its retail customers. And that creates an interesting tension of where is the real value in additional information? Is the additional information getting transparency in what the central bank is doing in terms of monetary policy or gaining information into how users use currency?

And we’ve seen this in private institutions already. We’ve seen innovations in the private payment space, say Venmo, trying to gain more information, more data about its users’ transaction records, thinking that data is valuable. I wonder if a CBDC could also offer some value in terms of generating more data about how customers use a given currency, and whether that would improve monetary policy or not.

[23:55] The tension there, of course, is perhaps consumers, retail customers don’t want to give all that data away to their government. Certainly in the private digital currency space that’s one of the big concerns of why we want cryptocurrencies perhaps as opposed to central bank currencies. I think that creates an interesting tension about how do we design central bank digital currencies in a useful way that will actually be adopted privately.

**Eugene Leventhal:**

Richard, did you want to jump in?

**Richard Brown:**

[24:24] Oh, yeah. Earlier you touched on three things, which I think are critical. And something I’ve been thinking about as well is that in the traditional financial world, there are checks and balances, there are regulations, there are committees, there are meetings, and all the rest of it. And that creates a certain pace of innovation, a certain buffer exists there.

[24:42] Where actually something’s going horribly, horribly wrong. People can see that train coming at them very slowly, presumably, and take steps to correct those systems. Are we moving into a world where those risks are potentially accelerated? Does the CBDC allow these central banks to get access to that data that you talked about and then potentially starts doing some A B tests, and doing some tweaks, and then handing things over to smart contracts?

[25:10] And then we potentially begin to face these risks where rapid experimentation, or maybe even real-time, or near to real-time monetary policy gets implemented. Is that a good thing, or is that a bad thing? Does this group have any ideas about that?

**Ariel Zetlin-Jones:**

[25:24] I view it as we usually think of more information as a good thing. In today’s world, especially in the US we’re seeing this advanced opening of the macroeconomy, and we’re seeing lots of choke points in different consumer goods, and that’s leading to very confusing perspectives on what’s happening to overall prices, which is the key objective of the central bank.

One of their two key objectives is to manage overall prices. Would having big data on a CBDC improve that in some meaningful way or not? I think that’s the perspective I was trying to add, question that perhaps the CBDC gives them more information, but does it come with other costs? And one of the costs, there’s a very old debate about discretion versus commitment in monetary policy.

[26:06] And Andrew was saying, perhaps we want to tie the central banks’ hands, tie them to the mast to pursue their policy, but maybe that’s costly because it doesn’t let them react in the ways where discretion could be valuable. I don’t have concrete answers for you, Richard, but I think that’s sort of the tension I was trying to get up.

**Andrew Miller:**

[26:25] I think there’s a very big risk of privacy falling to the wayside. And so I want to try to give a perspective here that really comes from… We worked through some of this in that CBDC design choices paper, and, really, the insight is just to recognize how open-ended the design space is, the scope of what you can do in terms of defining monetary policy, and defining your disclosure or privacy rules.

Nothing is baked-in from scratch, with a clean-slate design you aren’t constrained really in any way, what you can do with blockchain technology is quite flexible. I think that a lot of privacy mechanisms that we have, even checks and balances and privacy today, aren’t the result of design, they kind of happened by happenstance or are coming from the legacy institutional separate silos.

[27:23] You see this not only in finance but in things like fingerprint databases, where, just by having evolved separately, different government agencies, for example, don’t have compatible database formats. And that translates into a sort of firewalling privacy mechanism, even though it wasn’t designed that way on purpose, it just kind of happened that way.

I think that there’s a risk of assuming that privacy will work well in the future in a CBDC, even if it’s not designed for it in the same way that some of today’s institutions provide privacy by accident. And I think that that’s not the case at all, I think that if there’s not a policy choice that says that privacy is a first-class requirement, or human rights require it, or statutes, or whatever requirement. And so that must be built-in.

[28:11] I think that there’s a risk of by default, all the data will be available for ease of visibility, which has great benefits of efficiency, but also potentially a bigger risk of data breach and all of that. My hope with CBDCs is that they do incorporate privacy as a first-class design and goal. And then select from all of the appropriate technologies from zero-knowledge proofs and other cryptography that might be employed to ensure that kind of privacy.

[28:43] But it’s not something that should be taken for granted, it’s not something that’s built into blockchains, for example, quite the opposite. If you use an off-the-shelf blockchain, it’s probably going to involve replication of all of the data, which is worst for confidentiality or the risk of data breaches.

**Eugene Leventhal:**

[29:00] I wanted to follow a thread that started getting alluded to in the last couple of comments. And part of that is exploring the question of what problem are CBDCs looking to solve because also to think about Andrew’s [question], you’re alluding to important design considerations. And I personally very much agree with the privacy one, and I know maybe if we have time, Philipp, can maybe give us some color on the EU-based projects with the ECB and how they’re thinking about some things.

[29:30] But I guess to start off, what do you think is the core problem that something like CBDCs are solving and on the back of that, what are the important things to keep in mind to make sure missteps aren’t taken with a new technology experimented for those use cases? Ariel?

**Ariel Zetlin-Jones:**

[29:53] Well, I can speak to what people are proposing. And I do think there is a tension that our current payment system does not work perfectly. International remittances are very expensive, there are lots of unbanked individuals and households say, even in advanced economies, like the US. And so I think there’s a perspective that somehow CBDC might be a solution to that.

There’s a slightly more cynical take, which is that there’s a role to preserve monetary sovereignty, that if a Facebook creates a digital currency that could pose a risk to say the federal reserve in the US, and their ability to manage prices and employment in the economy. Which of those is the right perspective, I’m less clear about. I do think there’s a fundamental kind of challenge in answering your question, Eugene, which is, if we believe there’s this demand for private digital currencies, that’s one thing a central bank can’t compete with, right?

[30:49] If the goal is “I want a currency that’s not issued by a central bank,” then creating a Central Bank Digital Currency is not going to resolve that problem, right? The way to resolve that problem is through traditional regulation and to basically ban owning these currencies. And so I think we need to get at a core source of what is the demand for digital currency private or central.

[31:10] And as Philipp alluded to in the EU case, especially on the business side, [this is] why there’s demand for new types of Central Bank Digital Currency, that is not just “we want something not issued by the central bank.” And so I think you have to resolve that issue in some way. I’m curious to hear what Philipp thinks.

**Philipp Sandner:**

[31:27] Interesting perspective. And I also agree, I would actually add two more points here. I think there is some kind of international contest going on between regions, between countries. And I think there is some kind of contest or competition going on between potential other forms of managed monies potentially also including Bitcoin, right? We see just happening in El Salvador, right?

There is some kind of competitive pressure, and I think central banks have had a monopoly for issuing money and controlling monetary policy for quite some decades. And this is now being contested, I would say so by Facebook’s project Libra, by the Chinese Central Bank, which is really pushing these topics now, they’re basically launching next year apparently. Then we have potential competition coming from decentralized currencies, that’s the case of El Salvador’s Bitcoin.

[32:23] And therefore, I think central banks now will find suddenly in a space where they feel, maybe they don’t know it yet, maybe we all don’t know it yet, but there is a feeling out there that in the future payment might be different. Because at the end of the day, we as citizens would like to somehow keep our purchasing power. I can store gold, I can store Euro, I can store dollars with francs or bitcoin, at the end of the day, I don’t really mind, but I would like to be able to purchase my daily food and my rent. And I would like to keep my purchasing power for the future.

And in case central banks cannot deliver this in the future, then I think there is a, let’s call it threat, but it could also be a chance that citizens are turning away from this. And I think we should keep this kind of competition or contest in mind, which is in my mind now starting, and this contest could go on for the next years or maybe even decades.

[33:22] And another point I would like to make is the following, with CBDCs, and now I’m referencing the Chinese version. They are now trying to build a solution where you can transfer the money across cities, persons, even across countries within a couple of milliseconds, right? Given the speed of the transaction is some kind of competitive relevant metric, then suddenly, for example, take an international corporation such as Siemens, maybe Siemens chooses to onboard to the… Siemens as a German company chooses to onboard with the Chinese system, because then they can transact money around the world within a couple of milliseconds, whereas they cannot do it in Europe, for example.

The competitive pressure of the performance of payment infrastructures can also drive central banks to move towards CBDCs. Another facet here would be programmability, in case one central bank or one currency is providing programmability for financial constructs and capital markets, or for devices in the economy of things, in case companies are demanding this programmability, then they would like to have it.

[34:38] And in case, for example, the ECB is not providing this, then they turned towards the program of the stablecoins, or towards the program of the US dollar, or for whatever currency out there, because they might want to have to programmability. Because suddenly the programmability becomes one performance criteria, where their currency in a central bank has to perform and deliver.

[34:59] And therefore, I think this could be a new area of competition, which is going on. And we see this with Facebook’s project Libra or DM, actually nothing happened here, right? They have a technical infrastructure in place, they have done a lot of PR and work in whitepapers. But at the end of the day, right up until now in the last 2.5 years, not much happened in terms of real action and real solutions, right? But still, central banks are really kind of upset, they are now really investigating this topic and that’s in my mind has been driven by Facebook project 2.5 years ago.

**Eugene Leventhal:**

[35:41] That’s really interesting to think of how those competitive pressures might be getting more groups to be thinking of this, and then directly… then having a problem to solve that this is the best solution for, but Rich, I know you wanted to jump in?

**Richard Brown:**

[35:58] I think that, Philipp, you’ve identified something here that clarifies it for me is that we were dealing with different groups of stakeholders. We have the state, we have industry and we have retail, and they’re going to come at this with different requirements that potentially are challenging. And when it comes to proponents to CBDCs, the state or the central banks, there are certain narratives, and it feels like they’re narrowing in on and they run a spectrum.

We’ve seen, well, just this morning, Elizabeth Warren said that cryptocurrencies, I’m going to paraphrase here, are run by a shadowy cabal of super coders and miners, and that’s bad. And so therefore CBDCs can fix that problem. The other narrative that seems to be testing the waters is inclusion. And that’s been sort of this byline of crypto from the earliest days is this notion of banking, the unbanked.

[37:02] And there’s maybe a certain irony here that the banks are not talking about banking, the unbanked that they didn’t bank in the first place, but is that a compelling narrative? Does this group think that inclusion is potentially one of the benefits of a CBDC? Is there a likelihood that more people get bank accounts in this new world?

**Andrew Miller:**

I think I have an answer to that, I want to build on the comment about where programmability fits into CBDCs, I mean, I think that the structure of central banks is quite interesting. When I was getting into how cryptocurrencies work and then learned about finance just by some low-quality YouTube videos is very simplistic, like central banks are just central, but there’s really a lot more to it.

[37:24] I mean, they actually are kind of closer to DAOs, in the way they’re organized, there is a central bank organization, but member banks and commercial banks as part of them have a lot of sway. It’s a lot more nuanced and complicated than that. And what I think this fits into is, I think that there is room for a really nice design of what I think would be called a hybrid in CBDC, and this is kind of just expanding on this notion of CBDC as a platform.

I can imagine that the central bank would essentially act as a platform and set some bare operating rules, maybe some system invariants, like, no programming error for an application, will be to inflate in an unbounded way the base currency that the central bank is supposed to be managing. But in much the same way, like in the Ethereum blockchain, the rules of not printing more Ethereum or no EVM smart contract, you could write can inflate the amount of Ethereum currency it’s built, that is an invariant built and maintained at the platform level.

[38:53] I could imagine that the central bank would define some base rules like that possibly for safety, possibly for regulation, possibly for base monetary policy. But then what a programming smart contract interface could do is leave it up to the member banks to be really flexible in terms of what kinds of extra functionality they define, or monetary policy for their own tokens that are backed in some way by the central banks base way or money.

[39:21] There’s really quite a lot of flexibility that’s available there. I kind of imagined that may shape out into the role that this plays, where the member banks are responsible for the innovating and that takes place in a programming layer of the infrastructure. The central bank is responsible for setting safety rules, or they regulate ability rules, or even just fair play rules. And that those would be enforced at the protocol level. I mean, that seems to me to be the most… I don’t want to say, I can guess that that’s the most likely, but somehow that structure just appeals to me and kind of makes sense.

**Eugene Leventhal:**

[39:55] And I know we’re getting close to time, so I’m going to let Ariel respond and then just ask a final question before we wrap up.

**Ariel Zetlin-Jones:**

[40:05] I also want to follow up on Richard’s question, which is, if we look at the experience in monetary policy, where digital currency has been extremely successful, say in an emerging market like Kenya with M-Pesa, where it was a digital currency filling a role where there’s a lack of institutions and infrastructure for doing payments services, especially not within a village, but across the villages or across the country.

[40:30] There we saw a lot of success and I think it was natural it came out of a private company, right? The cell phone providers, because they had established the technology to allow for these transfers. It didn’t quite make sense for the government to take on this new role of creating a whole new infrastructure to allow people to do better payments services.

I think it’s a very different question when we look at financial inclusion say in an advanced economy like the US, right? We have to really have a deeper understanding of why we have a large group of unbanked people in the US, right? If they’re unbanked because they don’t want any records of themselves, then we have to ask, and this goes back to Andrew’s earlier point, right? What are the right design choices of a CBDC? And is that consistent with the US Government’s willingness to create totally private currency?

[41:18] You hear a lot of this Treasury Secretary Yellen said this early on in her tenure, recently that I don’t like cryptocurrency because it seems only used for nefarious purposes… and [this] is paraphrasing. And you sort of ask, well, how do you feel about cash then? Because that seems to be the predominant use of physical currency these days also. I wonder about this tension of what is the US willing to do in terms of a regulatory anti-money laundering, Know Your customer protocol for a Central Bank Digital Currency, and will that provide the privacy and security that the unbanked may want, if that’s the reason they’re unbanked.

[41:52] Again, in emerging economies, I understand why folks are unbanked, right? The infrastructure and institutions are not there. In advanced economies, I think it’s much less clear. And so when you ask, why is the Eurozone or the US creating CBDC for financial inclusion? I think it’s a much harder case to make. I’ll stop there and leave us time for our last question.

**Eugene Leventhal:**

[42:13] just wanted to follow up with, I mean, just building on a number of statements that all of you have made, given kind of some of the current pressures that are in existence for a variety of reasons, but there’s a bit of this race to roll out a CBDC. Some might be from a certain perspective potentially vying for establishing the digital future reserve currency, in a way we don’t need to speculate on the specific

[42:39] But given all that has been mentioned in this panel so far, from a citizen’s perspective, what should we be most worried about as central banks rush to figure out these new technologies and potentially deploy them? Do you have any specific concerns that are top of mind in your minds as these get rolled out?

**Philipp Sandner:**

[43:06] Well, I think privacy is the number one, privacy, privacy, privacy. We should as citizens try to force the institutions to keep privacy that might not necessarily be for all kinds of transactions. At least, like transactions below a specific threshold should be private the same way as we have a paper-based money, which is also private.

And the second point is monetary policy can become dangerous because for example, in Europe, we have negative interest rates, right? You are putting money on the bank account, and one year later you have less money on the bank account because we have negative interest rates. A negative interest rate can be pushed through much easier with digital infrastructure.

[43:50] And there is also a threat of money which can expire at some point of time. So you have to spend it otherwise it’s for whatever reason gone like a voucher. And there are a couple of design choices, where I think we have citizens, but also the political parties and those people who are let’s call it building or driving or governing the systems, should really be warned that we should not have a technology which would allow this.

**Eugene Leventhal:**

Andrew.

**Andrew Miller:**

[44:17] Yeah, I agree with the way that you put that and my concern is that there may be a tendency to think that because the design includes blockchain in some way, that that solves the problem of providing privacy for the individuals and accountability for the people running the system. But that’s not a built-in guarantee at all.

[44:37] It’s entirely possible to design a system that includes blockchain technology, but gets it backward, providing opacity and the ability to delete data or freeze accounts, roughly unaccountably for the administrators. And that provides no privacy for the individual users. You can’t just rely on technical destiny to assume that that’s going to carry out the right way, I think is really important to ensure that the designs that we have from the beginning reflect what we should be asking for in terms of rights to the citizens.

**Eugene Leventhal:**

Thank you, and Ariel, any final words before we wrap up?

**Ariel Zetlin-Jones:**

[45:20] Not to sound like the nerdy macroeconomists here, but just to point out everything Philipp said, academic economists might say are exactly a good thing. In theory, there’s nothing wrong with negative nominal interest rates. A zero lower bound is a constraint on monetary policy, alleviating that constraint is good. The experience in the Eurozone has not been great, so I appreciate Philipp’s perspective.

[45:43] A hot money where you get vouchers that expire can be a very valuable tool precisely say, in the midst of the pandemic. Overall, will that be used correctly by policymakers? We should be worried. Just to be a little concerned that it might enable the policy space in good ways, could it be used in the wrong way? Absolutely.

[46:02] And I agree broadly with the point that we need to deeply understand what is the desirable level of privacy in developing these digital currencies and our consumers, our retail, our citizens getting the appropriate mix of privacy and security from governments that they’re issuing.

**Eugene Leventhal:**

[46:23] Great. Well, we really just want to thank you all for taking the time to share your thoughts, opinions and work today. For those who want to continue the conversation beyond the single recording, please feel free to check out the Smart Contract Research website, [smartcontractresearch.org](http://smartcontractresearch.org/), where we’re going to have a dedicated post to this panel, that post will include more links to the work of all of our panelists, how to get in touch.

[46:49] And also some broad information on this topic as a whole. I mean, there’s so much, we, unfortunately, did not have a chance to dig deeper on or bring up. I definitely hope this is the first of many dialogues we’ll be having around this topic. And I just want to thank you all again and hope all the listeners have a chance to enjoy the rest of the summit.

**Andrew Miller:**

It’s been a blast, thanks for having us on.

**Ariel Zetlin-Jones:**

Thanks a lot.

**Richard Brown:**

Thanks for listening everybody, we really appreciate it.

**Philipp Sandner:**

Thanks

## Learn More About SCRF

The Smart Contract Research Forum (SCRF) is a grant-funded organization dedicated to advancing research while serving the web3 space. [Learn](https://github.com/smartcontractresearchforum/docs) more about SCRF, and discover ways to [get involved](https://github.com/smartcontractresearchforum/docs/blob/main/en/content_connecting_with_scrf.md).
