# SCRF Privacy and SNARKS Panel Transcript

The [Smart Contract Research Forum](https://www.smartcontractresearch.or****g/) (SCRF) has created a Privacy and SNARKS Panel Transcript for those interested in zkRollups to learn about their applications, designs, and research developments.

## Transcript

This is the transcript from the Privacy and SNARKS panel that was organized by SCRF as part of the Smart Contract Summit. To read more about the panel, the panelists, and the topic, refer to the [forum post](https://www.smartcontractresearch.org/t/smart-contract-summit-2021-privacy-and-snarks-panel/622).

**Eugene Leventhal:**

All right. Hello, and welcome to The Smart Contract Research Forum’s panel on privacy and SNARKS [Succinct Non-Interactive Argument of Knowledge], and we have some great guests here today to dig into the topic. I’m Eugene Leventhal. I’m the operations lead here at SCRF, and I’m just going to quickly hand it off to Lucas Nuzzi, who’s our research lead, to moderate and lead this discussion. So yeah, please take it away, Lucas.

**Lucas Nuzzi:**

[00:32] Thank you, Eugene, and welcome everyone to what’s going to be a really fun discussion on the state of industry when it comes to ZK-rollups [Zero-Knowledge] and the low-level protocols that enable them. And to have this conversation, we have two of what I consider the top researchers in this space doing work in this area. Ariel Gabizon who has been doing research in this area for quite some time, now at Aztec Protocol who’s building a really interesting ZK-rollup solution as well as Aleks Vlasov, who has also been researching this area for quite some time and has been working with ZK Sync in their various approaches to rollups.

**Lucas Nuzzi:**

Gentlemen welcome to the panel. Really a pleasure to have you on board. Maybe to kick things off you guys can give a little bit of an introduction of yourselves and your projects. And we do have some questions to go over, but it would be great to hear from you guys the evolution of your research, what you’ve been working on, and the areas that you focus on, maybe starting with you, Ariel?

**Ariel Gabizon:**

[1:54] Yeah, sure. Basically, I spent a lot of years in academia doing math and computer science, and once basically I read the bitcoin white paper, I felt that I should get into this world, and the best way for me to do it seemed to be through these ZK zero-knowledge proofs since they were relatively math-heavy with the sort of math I like and was comfortable with. So that led to me working with Eli Ben-Sasson back in Technion University in Israel in the early days of STARKs before they were called STARKs. Then I left academia to work on Zcash, the first trusted setups. The first commercial use of SNARKs was there and that was really exciting.

**Ariel Gabizon:**

[2:54] Yeah, and then sort of a chance meeting with Zach Williamson led to this universal zk-SNARK called PLONK [Permutations over Lagrange-bases for Oecumenical Noninteractive arguments of Knowledge] which I think really put universal SNARKs in the practical… made them very, very practical, and then that led to me moving from Protocol Labs where I was working to Aztec to focus on this work with Zach and the Aztec team.

**Lucas Nuzzi:**

Excellent. How about you, Aleks?

**Aleksandr Vlasov:**

[3:35] Oh, well regarding the way into SNARKs themself, I was participating in ETH protocol. I think it was actually this first one from ETHGlobal series, which continued for a few years after. At this hackathon there was the talk well first by, I think by Vitalik on SNARKs, and then by Eli Ben-Sasson on STARKs. So this is when it first caught my attention in general for what’s possible to do with the SNARKs at that point in time. Then I was working on Plasmas in different flavors. Then at some point, we decided to form Matter Labs to bring the best from two worlds and marry the rollups and zk-SNARKs to make the ZK Sync, the zk-Rollup released a few years ago.

**Aleksandr Vlasov:**

[4:27] So now we are continuing to develop it, to bring a version 2.0 and it should be able to run user-defined smart contracts which should be compilable from Solidity and Sync, which is our developed programming language. Also, not specifically for circuits, just normal programming. In theory, we should be able to even build RUST and run it in our architecture, but it’s always a bit off-topic. So yeah, along the way I participated in improving SNARKs as for us it’s more like a tool than something like pristine and fundamental. So for this purpose, we developed… We published a small paper about the transparent polynomial commitments which used FRI, and then which led into the expanded paper called the RedShift. It was roughly my way into here, and now we’re in the final stages to bring ZK Sync 2.0 with smart contracts to life with basically all SNARK-related work done.

**Aleksandr Vlasov:**

[5:42] Now we just have to check the code, run the tests and be able to release it so people can try a compiler, see how the VM was designed. Actually, we have to write a lot of manuals, but it should lead us on a good track.

**Lucas Nuzzi:**

[5:59] Yeah, super interesting background. I think it ties things very nicely. I do remember when Vitalik first described what we now call zk-rollups, essentially applying this technology which the industry had predominantly seen as an approach to privacy with projects like Zcash applied to scalability, right, enabling transactions to be processed outside of the blockchain and essentially borrowing some ideas even from Plasma at a time when more research was coming out on the feasibility of Plasma that I would say disappointed a lot of people.

**Lucas Nuzzi:**

[6:42] So to set the stage a little bit, it’ll be interesting to talk about the commonality and the theme of the projects that you guys are working on because when people think about zk-SNARKs, they still have this anchor towards privacy, right, whereas because a lot because of the research that you guys have produced over the years, that theme has shift quite a bit, right; from privacy to scalability. Now with recursive SNARKs with the ability to program contracts using these systems and still carrying some other benefits that SNARKs intrinsically have. So maybe to set the stage a little bit, Ariel, could you just talk about recursive SNARKs and PlonK and what is it that enables these contracts to be generalized and really just granting the tools to the developers to build these contracts using this technology?

**Ariel Gabizon:**

[7:51] Well, so maybe one thing to mention is why are recursive SNARKs relevant to, or essential to programmability, and I guess one part of that is if eventually, you have one sort of verification contract that is constant, like say this is the contract that verifies the rollup. So this contract is fixed; it’s not dependent on a specific program. So in this sense, recursion helps you because whatever you’re actual circuit is, the final program you’re running is just a verifier.

**Ariel Gabizon:**

[8:55] So, what is the relation between PlonK and recursion? So the first thing to notice is that, in principle, any zk SNARK gives you recursion because zk-SNARKs allow you to approve statements about any program. So you can always prove them, prove a statement about the SNARK verification program in particular. So recursion was never impossible theoretically. It was really a question of constants and the concrete constants when writing your program, your SNARK verification program, due to basically field mismatches, we’re just very large. So one reason why PlonK made recursion more simpler is basically shaving off a few constant factors in terms of representing constraints compared to the R1CS [Rank-1 Constraint Systems] representation, and these factors shaved off exactly sort of… made this writing the recursive verification program more practical without the need for any special tricks elliptic curve cycles.

**Ariel Gabizon:**

Yeah, so I’m saying a lot of things there that maybe need explaining, but that’s sort of the mid to high level.

**Lucas Nuzzi:**

[10:39] Yeah, no absolutely, and I think part of the priming that I see exists when people reason about zk-Rollups, I think it’s exactly that, right? I think there’s a lot of priming in terms of applicability. I think there’s this idea that a zk-SNARK is application-specific, right. Its role is to simply verify transactions, and the reason why I think there’s been a lot of this priming is that in order for you to, under previous systems, bootstrap an application, it requires creating this string through a process that must generate a random number, a random string. What your research has shown over the years is that this is abstracted away through shaving some of those parameters so that you can apply this technology to broader programs without the requirements of actually regenerating these strings which increase the potential attack vectors of these systems, right.

**Lucas Nuzzi:**

So it really just enabled a way for you to reuse that SRS for a plethora of applications that can then be granted the benefits of this technology. Is this a correct characterization?

**Ariel Gabizon:**

[12:20] So that is another huge issue, yeah, that universal SNARKs like PlonK don’t require a setup per circuit. Yeah. I was referring to this I guess other more low level issue to actually write the SNARK verifier is a program you need to simulate these field operations in a non-native field, and that was extremely inefficient before Plonk. But actually, maybe you’re right that for… Yeah. Actually, you’re right that a much more basic issue, if you want recursion and user-defined circuits, yeah. So the universality is actually a much larger and more basic point, yeah. Otherwise, every user would need to run their own trusted setup.

**Lucas Nuzzi:**

[13:33] Yeah, and I think there’s been a lot of really interesting content, and I think even the initial Powers of Tau Ceremony from Zcash that you were one of the architects of, I think there’s a lot of mysticism around what that actually entails and how that is performed, but the basic idea is that string must be secure enough or random enough so that you have guarantees around the provers and verifiers of these systems.

**Lucas Nuzzi:**

[14:16] Aleks, you’ve worked on this scheme called RedShift, which was a really interesting piece of research. It basically introduced an interactive Oracle proof system that used polynomial commitments to essentially circumvent the need for a trusted SRS. Could you talk a little bit about RedShift? What motivated that research? Was it the security and more universal angle that motivated that research, and also, if you could also talk about the evolution of that research and what led you guys into PLONK as that research evolved and maybe the tradeoffs associated with that research?

**Aleksandr Vlasov:**

[15:18] Well first of all I should mention that there was like, for RedShift and its histories, there was no particular decision to do such research. The historical status this time was that there was a DEEP-FRI paper by Eli Ben-Sasson and his colleagues which basically used FRI proximity tested protocol in some particular way which allows them to have more efficient STARK. And here, by STARK, I mean the proof system and the way your arithmetization which is called AIR in the original paper. Basically what this paper was doing is very close to what the PlonK paper was doing in its original form with just the polynomial commitments which are architect commitments. Basically, the prover commits to the set of polynomials and then draws around the point. Then make a standard trick of quotient. Basically, if your polynomial is at this value at this point, then you can perform a division, formal division operation, and that the result will also be a polynomial.

**Aleksandr Vlasov:**

Then they used the FRI to prove that this result of the division is indeed very close to polynomial which was sufficient for all the purposes of STARK as a proof system. But it was never called a polynomial commitment. Even while it was doing basically the same as the commitment itself, just in a different way. I read this paper, and then I took half a year or something like this. There was a PlonK paper, which I seen was covering largely the same details in a same format, and only then I just randomly in a train actually had an idea; well, this is basically the same and why no one tried to do it. Then we spent two weeks trying to convince ourselves that there was no, some trivial mistake and overlooked that this is very much the same idea which was never covered.

**Aleksandr Vlasov:**

[17:31] So then we made a very small paper on archive which was basically talking about the polynomial commitments, which was treat commitments to only a single polynomial and used FRI as a proximity tested protocol in a mode which is called unique decoding radius. A little bit simpler, it was testing that something which prover gave you is close to the polynomial. It’s very close to polynomial. Let’s call it this way for simplicity for now. Which led to larger proof size, which was a problem with our original STARKs back then when they were introduced. They required very small radius for testing of proximity which led to larger proofs.

**Aleksandr Vlasov:**

[18:19] Then we decided to go beyond this, the same achievement which was done in the DEEP-FRI paper to go beyond unique decoding radius, and this was done in the RedShift paper. The main trick or/problem with going beyond decoding radius was that now the prover is able to commit not just to a single polynomial but some set of polynomials. The set is still small compared to the field size. So it wasn’t the end of the day for soundness, but it would be okay for witness polynomials. So the prover can give you something which is like maybe one polynomial out of 10, which satisfies the verification relationship, was still fine for witness polynomials, but it would be a problem for set of polynomials which were present in all the proof systems as in some STARKs and others which are for uniform circuits. Let’s not go that deep into this direction.

**Aleksandr Vlasov:**

[19:26] So we have to find a way how to actually pinpoint a single polynomial out of the set at the setup time, which was done in RedShift, which basically brought the best from the STARKs world and basically transferred it to all the protocols which required polynomial commitments. That’s why it was demonstrated on Quant itself because it was first an original inspiration and then the idea was if you can do the same, you can run the same proofs by just swapping the commitment scheme and maybe adding some factors in the soundness. So that’s why the RedShift was made in a form which basically taking the PlonK and change it a little bit.

**Ariel Gabizon**

[20:28] Yeah, so actually, Aleks, what do you think really about the non-preprocessing STARKs versus doing RedShift? If you had to choose between these two, what would you choose?

**Aleksandr Vlasov:**

[20:50] Well, I have a preference for one with the preprocessing for reasons that it can be a much simpler to write and design by people who cannot just take the polynomials and write a polynomial protocol by hand on a piece of paper by basically linking all the weakness values by themself in a very large set of weakness polynomials. So the problem with the protocols, which are like STARKs without preprocessing, is that your set of constraints is so much non-trivial that first of all it’s difficult to design without mistakes and the second after you design it, it’s unlikely that you will find another person who will be able to review it.

**Aleksandr Vlasov:**

[21:30] But if your proof system is more universal in a sense that the preprocessing written ones does everything for you, and when you design the circuit you only write a code which is much simpler. So you do not manually take care of which variable is located in what polynomial at which index, and you basically treat them like values and variables in any… in some convoluted programming language. It eliminates a lot of mistakes, and it actually becomes auditable and understandable by the wider audience. That’s why I think that there are more people which are able to write a long circuit or maybe understand… like to understand sprouts or supplements Z-cash circuits than people who would be able to write a STARK to, for example, do the Pederson commitment. And Pederson commitment was actually quite trivial.

**Aleksandr Vlasov:**

[22:39] For whatever people in StarkWare did for the Cairo programming language, I can guess how it works. I didn’t look in details and didn’t try to reverse it, but I can guess how it works, but I think it would be non-trivial for anyone to try to write an external manual to how it’s actually implemented. Even so, you will see a full set of constraints in the verifier if it’s implemented as a Solidity contract.

**Lucas Nuzzi:**

[23:13] Fascinating. Yeah, it’s interesting to hear about the reasoning behind some of these straight ops, right. I think if the research around even more recently with PlonK and its newer iterations, and all this predecessence showcases is that there are some non-trivial tradeoffs at play when it comes to usability, proving time, verification time, proof sizes, even complexity. What other tradeoffs fuel your research as you’re thinking about, for example, shifting the commitment scheme in this circumstance for efficiency purposes? What are the tradeoffs that influence your research, especially as you’re trying to build the system for Ethereum applications?

**Aleksandr Vlasov:**

[24:24] Well, I think once you actually separate two-part here. One is designing the final system in a sense that what circuits you write, which is the functions of the circuits, whether those circuits require some recursive verification because they prove different substatements of one larger logical statement. So they require recursive verification. Another tradeoff is purely regarding the proof systems and concrete implementations of the recursive approach. For example, if you take the Fractal paper, it was a direct comparison was done there. So the Fractal paper is also transparent SNARK or STARK, however, you want with the preprocessing.

**Aleksandr Vlasov:**

What they did is they presented the size of the circuit which does the verification, a recursive verification of single statement. If you use one hash or another hash to construct the numerical trees when you do the proofs. So if you use a standard non-algebraic hash, then your statement… because then your verification circuit is very large because non-algebraic hashes take a lot of constraints to implement, which was partially solved by the PlonK with low cap tables. We can cover it a little bit later. Another example they did, and they used the rescue hash as a hash to construct the Merkle trees which led to much smaller circuits to implement the verifier, but which also led to the much larger proving time because the hash itself was very slow to compute.

**Aleksandr Vlasov:**

[26:06] So this would be I would say I think more to the question of which you asked originally in the sense of different tradeoffs. In a similar direction, you can view how many constraints does one recursive aggregation in PlonK take, and it also depends a lot… for example, if your verification keys are all the same, it’s one number. If your verification keys are all different, it’s completely different number. I think five times, larger if I remember correctly. Roughly, at least. And this even would not be a complete verification; it would be aggregation, which is also a little bit different procedure, and Ariel can cover it in details, I think, much better than I do. So for this, we should separate this talk and first maybe talk about the proof systems and tradeoffs coming from proof systems themself, and then you can try to talk about how you can actually try to implement a programmability separately, and which is unlikely to depend on what proof system you take if you have the recursion. It’s another field of optimizations I would say.

**Lucas Nuzzi:**

[27:22] Yeah, that’s a very interesting framing. I think that’s exactly right. You start with the proof system and then recursion is applied, and then you have all the interesting benefits of it. But Ariel, were you going to say something?

**Ariel Gabizon:**

No. What was I going to say?

**Lucas Nuzzi:**

I guess, do you agree with this framing? Is this the correct way to reason about the trade-offs of these systems?

**Ariel Gabizon:**

Well, what is that way again?

**Aleksandr Vlasov:**

[28:03] was more about that you can separate this large equation made by Lucas into one. It’s like what are tradeoffs in proof systems and their particular implementations versus a design area of how we actually implement programmability. And from my perspective, it’s also completely two different tasks. One is optimize how you implement proof systems and recursion, like particular hash function choices, commitment schemes choices, maybe something else we can talk about this. And another one is how you actually make a circuit which, for example, does a zk-Rollup. And maybe with verified user-defined circuits and contracts. So I would say two completely different deals for me at least.

**Ariel Gabizon:**

[28:55] Yeah. Well, one thing just I think about your, Lucas, originally you… In terms of tradeoffs of polynomial commitment schemes, that I think right now the KZG, the Kate-Zaverucha-Goldberg one is clearly the winner. I think the only reason to use anything else is if pairing-friendly curves will at some point be crushed and, yeah. Then there’ll be no choice but to use something else. Yeah, I don’t know. I think there are a lot of parts of this question. Yeah, maybe let’s go to the next question. There’s a lot of parts so I’m not sure what to [crosstalk 00:29:57]-

**Lucas Nuzzi:**

[29:58] It’s a loaded question. But you did mention something interesting with regards to pairing-based cryptography that we’ve had a couple of discussions in the past, and you of course, whose topic of your research is security. Ethereum uses a variance of BN256 as a proving curve or as a curve at the base layer. Eth2 moving to BLS12-31, what is your take on the security of these curves and maybe of pairing-based cryptography more generally? Do you think there will be a scenario in the short-term, and here’s another loaded question, where these curves need to change or the setups need to change?

**Ariel Gabizon:**

[30:53] Yeah. I don’t know. It’s like asking will Bitcoin hit one million dollars, or let’s say, will Bitcoin hit $100,000 within three months, two years, five years, never [crosstalk 00:31:07]-

**Lucas Nuzzi:**

[31:11] Is it a matter of when not if?

**Ariel Gabizon:**

[31:16] Well, there is a question of if. It’s really hard to say. You’ve got these number field save attacks that are what makes us go to larger curves, and it’s really tricky to say. You occasionally have a new paper with some improvement and then it’s like how fast are these improvements going to go? Are they going to get stuck? Are they going to… yeah. So it’s really hard to say. I mean I try to understand practically how safe is BN254 for the next few years. Yeah, honestly it’s really hard to say. It’s really hard to say if like, okay, the current attacks need a little extra trick to make it dangerous to use BN254 or there’s going to be 10 years till this trick comes or it’s really hard to say.

**Ariel Gabizon:**

[32:34] One annoying thing is that when you’ve got the Pollard’s rho algorithm, so the proof run time is very well analyzed, but with these number field sieve attacks, they’re saying, okay, this is the run time under these number sort of theoretic conjectures. Then you’re like okay, so should I update my code according to the more pessimistic, pessimistic in terms of, say, the user not the attacker, should I update my curve according to the more pessimistic estimate sort of versions of these conjectures or should I actually wait till there’s a… right? So these curves have 200, 254 bits that we’re using right now in Ethereum. So if you look at Zcash, for example, they write… the minute there was a paper saying, okay, there is potentially an attack on this current, immediately they move.

**Ariel Gabizon:**

[33:42] So what should be your approach? The minute someone writes a paper where this maybe is not safe anymore, do you move then? Or, do you say, well show me an actual attack on… you know? You say, "Okay, Sha-256 is not safe anymore. It has what 80 rounds. Show me a recent attack of break 70 of the 80 round.“So equivalent, right, show me an actual discreet log computation in a field that is getting close to what we’re using, and then I’ll switch my curve.” It seems that the more what people are actually doing is the minute there’s a paper saying, okay, this may be dangerous, they immediately move. They don’t, they don’t want more evidence.

**Ariel Gabizon:**

[34:28] So honestly, yeah, sorry this is a bit of rant. When Zcash… when we moved so quickly, I was like, oh, we’re giving them too much credit.

**Lucas Nuzzi:**

[34:37] Legitimizing it too much.

**Ariel Gabizon:**

[34:30] Yeah. But on the other hand when I talked to some of these experts in the last few months, yeah, I don’t know, it seems like they have a lot of tricks up their sleeves and… So yeah, this is sort of a long way of saying I don’t really know. It really is like the price of Bitcoin, like how long will it take to hit the next like the 100K. Is it going to be soon? Is it going to be never? Is it going to be really slowly?

**Lucas Nuzzi:**

[35:18] No one knows. Yeah. It’s an interesting area of research, and I think it’s exactly what we said, right. It’s really a matter of making these design decisions on a proactive or reactive basis on the basis of how legitimate or how concerned from a practical perspective some of these attacks are. Claus Schorr recently said that he broke RSA [Rivest–Shamir–Adleman] and is the industry completely moving away from RSA. It’s not really happening. So it fits into those tradeoffs, but is this something that as you’re designing these systems that you guys take into consideration, do you have contingency plans if this were to happen? How proactive is that? Is that because I would imagine it would be a non-trivial shift, right, if pairing-based curves were to be, as you mentioned, that 70 rounds be proven susceptible to some of these attacks? Or is that now part of the-

**Ariel Gabizon:**

Well…

**Lucas Nuzzi:**

[36:37] Of those research decisions or design decisions?

**Ariel Gabizon:**

[36:42] Well, I think the nice thing is yeah, since the polynomial commitment scheme is an independent component, it shouldn’t be too tricky to move to a system that doesn’t rely on pairing-based curves. Yeah. You’ll take the efficiency hit, but it shouldn’t be too tricky.

**Lucas Nuzzi:**

[37:16] Do you have a favorite alternative to BN256 that maybe each two researchers should consider or even the client developers should be looking out for?

**Ariel Gabizon:**

[37:33] I mean just from the top of my head, I would maybe switch to these discreet algorithm-based systems. So something similar to what Zcash is doing with Halo.

**Lucas Nuzzi:**

[37:50] Yeah, which is another really interesting move, and you know uses. It’s interesting to think about the modularity of these systems and how research ends up intersecting. I know there’s quite a bit of inspiration from PlonK that’s being used within Halo which is super interesting. But in the topic of tooling, and it’s interesting to think about these systems interacting with base layers like Ethereum, like other networks, of course, we’re talking about the decisions that are made at the client level that impacts the design of this rollup solutions. What is your take on the states of tooling around these systems, especially as it relates to building and iterating upon efficiency?

**Lucas Nuzzi:**

[38:51] There’s been quite a bit of conversations recently about the Poseidon hash function that’s specialized for efficiency in the zero-knowledge system paradigm. Is this something that you guys are looking into? Is this something that you guys plan on integrating? Curious to hear your take about this, and tooling more broadly for the systems that you’re building.

**Aleksandr Vlasov:**

[39:23] Well, I can try to answer this question, the previous one in a little bit opposite direction. So for us, and we, for various reasons, we want to switch away from BN254. For example, because we built a rollup, we should be able to run the Solidity-based smart contracts. Then we get to support when the primitive type, like the people which would use, is 256-bit unsigned integer, which doesn’t fit into the base field of both BN256 and BLS12 through 81, and it’s not even clear if BLS12 to 81 will go into the Ethereum one point whatever in the nearby time.

**Aleksandr Vlasov:**

So for this reason, we really want to switch to another proof system. Well, not a proof system. By proof system, I would say it’s still going to be PLONK in a sense of how their humanization is performed, the setup, and the processing is performed. It’s just a commitment scheme of change. And for the Redshift style commitment scheme, we’ve seen quite a lot of actually good sides in there. So when it was originally introduced, we obviously would have the same problem as Fractal. If you use a fast hash function to make a proof, then your circuit size is going to be large to make a verifier. Then we got the PLONK with lookout tables which shaved a constant on implementation of all non-algebraic hashes, which made a verifier actually kind of feasible. Well not feasible, just quite small in there.

**Aleksandr Vlasov:**

[41:14] Then we actually got the Halo infinite paper, which touched the FRI-based preliminary commitment schemes very little, but which gave us inspirations that we actually overlooked a one trick. So instead of making a full verifier, we can, indeed, go into the aggregation direction. And the same way we can as in Halo infinite, we can perform aggregation and delays of final verification of proximity to the very last proof verification, which shaved a factor of logarithm from the complexity of the verifier circuit because we don’t… We need to do integration with a smaller number of hashes at the end of the day by the size of the circuit, which we want to recursively verify.

**Aleksandr Vlasov:**

[42:10] And now, from what I see, I would expect in the nearby time some new algebraic hashes which should be much faster to compute even compared to the Poseidon, which is the fastest one of which I know in which is secure, but it’s still not at the level of performance, for example, of Blake and Sha-256. This will allow us to make a verifier even smaller. So nothing will stop us from going to transparent proof systems and getting all the benefits. A field which we can choose freely which will be 256-bit unsigned integer in a single element. And in addition, we can make a field in such a way that our multiplication will be quite faster than over arbitrary prime fields just because of the structure of the field modules.

**Aleksandr Vlasov:**

[43:07] We can do a lot of other like combining all these tricks is a huge benefit, and this will basically benefit the final circuits which implement the virtual machine and the rollup itself. So for us, it’s actually a positive direction in this sense, and really you would want to switch for a lot of reasons. And the only thing which would require an extreme base level is basically the EVM384 set of protocols, which is still not strictly required but would be convenient.

Ariel Gabizon:

[43:44] So this 384 thing, it does have 256 UINT in a single field element?

**Aleksandr Vlasov:**

[43:54] Well I mean we can choose a field a little bit smaller since we had it in 20 bits, basically five 64 bit links to be able to utilize things like the lowest four links are going to be 000 and 1, a standard trick for faster Montgomery multiplication. Then we can also do a lot of partial Montgomery reductions which are actually very convenient for modern processors without branching and other stuff. So with all this, what we will need at the end of the day is basically perform some field operations in Ethereum’s smart contract when we will do the verification, like the one final verification in Ethereum.

**Aleksandr Vlasov:**

[44:41] It’s only there when we will need to have Ethereum being able to make modular operations and still we can do it with existing privileges but we will just pay more.

**Lucas Nuzzi:**

[44:56] This might be an interesting segue into this level of compatibility with Ethereum programs. I think one discussion that is… Well, there are two main discussions that are happening right now in terms of zk-Rollups that excite people. I think one relates to this idea where you can scale a lot of these applications as you’re processing it in a rollup layer and still being able to use the tooling, the compilers, the IDs that exist for a language like Solidity. Then also in the context of privacy, potentially having a pathway to having these programs being private.

**Lucas Nuzzi:**

[45:50] I think it’ll be really interesting for the audience to get an overview of how that is achieved, respectively, in your projects which differs quite a bit, but I’ll be interested in hearing from you guys, maybe starting with you Aleks, given your work on zk-EVM. What is zk-EVM? What level of privacy should users expect from zk-EVM? How did you guys go about designing it, and what are the interesting things that you’ve learned along the way? Then we can switch to you, Ariel, and talk about the bridges that you guys are building on Aztec.

**Aleksandr Vlasov:**

[46:40] Well, first of all, I should note, that zk-EVM has become for some reason a very popular term and is abused because the meaning of this is not defined. So just to make things concrete, the things which we designed when it was called the zk-EVM by us as the first who named it is that we designed a virtual machine, like a rollup, which obviously should integrate some form of virtual machine to be able to run user-defined smart contracts, and said we want to run 99.9% of Solidity contracts in the sense that we should be able to compile them. It’s not exactly the same as trying to claim that you would want to write an EVM bytecode and thematic compatible virtual machine isn’t implemented as a surrogate, which is completely different deal which I would firstly consider over the real complexity for various reasons and all the experience which we gained when we designed our virtual machine.

**Aleksandr Vlasov:**

So that’s why I would say let’s not use zk-EVM in a conversation because it will be very misleading. But for us, it aim is basically take the user Solidity code, compile it into the set of procreations which is supported by our virtual machine and which end-user may not even care as most people don’t care what is a Ethereum bytecode is and what are particular operations in there as long as their Solidity code compiles. Then you basically get all the same functionality with quite few extensions. So this is our goal.

**Aleksandr Vlasov:**

[48:37] Then, yeah, it obviously should be zero-knowledge friendly. So when it’s expressed as a circuit which proves the execution of user-defined programming, and this approach is not even new. It was in original TinyRAM paper from 2013, which allow you to execute basically RB3 user-defined program by simulating the processor. Yes, you can do the same now. You can just do it a little bit more efficient by shaving a lot of constants from the concrete proof complexity that itself is still not a new approach. So yeah.

**Aleksandr Vlasov:**

[49:11] And the recursion definitely helps us because we can now use the approach of divide and conquer. So for whatever logical statement we have, if this logical statement is highly heterogeneous, so it has some sub statements which are quite local and can be proven separately, we could efficiently prove those statements separately, and then perform a recursive verification which will also guarantee us that the full statement is also true. There’s the same approach… Well, this is I would say the only possible approach to make something which looks like an Ethereum but implemented as zk-Rollup. So yeah, we’re just moving into this direction. Almost done, and now we’re… We will share our experience as soon as we’re done writing the manuals actually. Yeah.

**Lucas Nuzzi:**

Catching up on some documentation. Yeah, that’s always helpful.

**Aleksandr Vlasov:**

[50:20] Well, the problem is we have the code very well documented of tested in various parts separately and together. The problem is that the computation itself is in the code in the sense that it’s in very large comments that have various things. So we cannot make a document which other people can read without going back and forth between the browser tabs. So we have to assemble it all together in one place and make something and make it a little bit more formal along with their obviously tooling compiler and way for people to be able to test it locally without too much pain and starting too many independent packages, et cetera, et cetera. So yeah, we have to polish it for users, even while it’s done as a fundamental work.

**Lucas Nuzzi:**

[51:12] And I ask about privacy because there’s quite a bit on miner extractable value that I think a lot of industry observers see as critical to be resolved or at least curbed in a lot of ways via better privacy-preserving solution. I was reading recently about the creation of Aztec and there’s a big motivation there for security tokens in the very beginning of the project, which obviously require a level of privacy for regulatory reasons but even beyond if you think about these systems processing real-world economic activity and some of the drawbacks in pseudonymity and account-based model. It is something that is of concern.

**Lucas Nuzzi:**

[52:12] What levels of privacy, maybe starting with you, Aleks, and then we can switch to the conversation on Aztec, but what levels of privacy can users of ZK Sync expect as this VM functionality is introduced?

**Aleksandr Vlasov:**

[52:29] Well for us, the superiority sequence was first we achieved the functionality in decentralization, and then we can start to look at the direction of privacy more closely. Then I would say the level of privacy is basically the same as in the layer one in Ethereum because user-defined programs are known to the sequencer. So whoever produces a block will know what programs he runs and also all the state will be known. Eventually, we will add an ability for users to verify their own zero-knowledge proofs in our system as a part of their program execution, and this will provide them the privacy that if you can do the same, you can verify the SNARK with some custom logic and now in history layer one, but it’s not there yet.

**Aleksandr Vlasov:**

So for now, the priority was able to run end-user contracts with the same guarantees in Ethereum and also achieve decentralization. So it means that state replication and that rollup data post into Ethereum as a public data, it all should be done in first release as the highest priority. And obviously, as exit mode, whenever the chain stops, we have a well-defined mechanism to be able not to just take out the funds but also to restart the chain at some point. Obviously in a valid state. So yeah, for us, the priority is later in time. But I think for Ariel it’s exactly opposite.

**Lucas Nuzzi:**

[54:27] Yeah, I think it’ll be really interesting to hear about Aztec’s approach, Ariel, in terms of first how is this kind of composability achieved with Aztec especially as it relates to DEEP-FRI applications, and then love to hear about what do you guys think about privacy, the privacy guarantees that users can expect from using your systems as they launch.

**Ariel Gabizon:**

[55:02] Yeah. So we took a privacy-first approach. Perhaps, to be honest, that also is a differentiating factor are so many talented smart people working on rollups. So right now, if you go to zk.money, you can just do transactions with Ethereum or di-transactions where amounts, sender, receiver are totally private. Our next sort of short-term goal is what we call the DeFi bridge, and that will allow you to call, say, Uniswap first of all in a much cheaper way because your fee will be split with all the other rollup users, and you will also get your call will also be private. So the amount that you deposit to, say, Uniswap will be public, but your identity is private. So basically, it’s a cheap and private way to access DeFi. That’s our next short-term goal, and we hope to have it out in the next two, three months on MainNet.

**Ariel Gabizon:**

[56:40] More long-term, our aim is to have what we call dark contracts where the sender, receiver, and also the code of the program or logic of the transaction, they’re all hidden from the chain. And the logic of the transaction is totally arbitrary and user chosen.

**Lucas Nuzzi:**

[57:12] Yeah, that’s a fascinating set of goals. Just out of curiosity from a data structure perspective, would it be analogous to, say a Zcash transaction where you have a special adjust type like from, let’s, for the sake of comparison, a shielded to shielded transaction using Zcash lingo. So you would not see amounts. You would not see the sender recipient pseudonyms and you have essentially a blob representing the actual opcodes of the application. Is that, at a high level, what that data structure would generally look like?

**Ariel Gabizon:**

[58:02] Yeah. So it’s similar to if people know the Zaksi paper, it’s similar to what goes on there. So if in Zcash, you have an encrypted version of your note with the address and amount on the blockchain. So for a dark contract, this encrypted note, it will contain amount, well asset type, address and it will also contain a verification key, which is what determines the logic of the transaction. Yeah, and again, what you have on-chain is just an encryption or hiding commitment of this data.

**Lucas Nuzzi:**

[58:52] Really, really interesting. One thing that I want to make sure that I ask you guys is that… So there’s been quite a bit of discussions right now with regards to the Ethereum virtual machine post the merge, which is what they’re calling this, process whereby IF1 is connected to IF2 as one of the shards of many shards that blockchain will support once the full functionality’s launched. Over the years there’ve been several problems, both in terms of usability and security with the EVM. It’s been described as not a great virtual machine and has motivated a lot of conversations about changing it to Web Assembly and other virtual machines that carry different sets of trade-offs.

**Lucas Nuzzi:**

[59:54] If that shift were to happen, how easy would it be for you guys? Is it modular enough so that in case there’s a change in the virtual machine that’s ultimately used in Ethereum that your systems can adapt to it, is this part of the design decisions as you’re building it, not to be strictly married to the EVM? And this is for either of you guys.

**Aleksandr Vlasov:**

[1:00:24] Well, it’s obviously modular in the sense that there is some state, a long-term storage, and there is what like… or what people take the EVM, it’s like a little extended state transition function. So the problem is at the moment when you have EVM as a virtual machine on Ethereum and Solidity as a defacto standard language to write the contracts for Ethereum. So we take in only language from this list, and the virtual machine for us is completely custom-designed just to be able to support everything which users want for their smart contracts. Gradually is starting in basically then having 99.9 contracts as our goal, maybe extend the nines later on.

**Aleksandr Vlasov:**

[1:01:13] So I would actually expect it in a different way that Ethereum itself, if Ethereum itself will ever reconsider to change the execution environment in a sense that change the state transition function and blast some other virtual machine data model and all other related parts, maybe that Ethereum should look at the zero-knowledge friendly virtual machines designs as a part of the separate to bring Solidity to the zk-Rollups than going to try to highly preserve the EVM semantics or try to follow Web Assembly, which was demonstrated to be not the ideal case in case if you try to keep other semantics of the EVM, for example. If your data type is 256-bit large, then, unfortunately, cannot efficiently manipulate the data, and it will be a huge slowdown.

**Aleksandr Vlasov:**

[1:02:27] And the same way for gas metering, for example, as it’s done now. When you pay for storage from the same gas resource as you send with the transaction, and you then you see that your storage accesses go higher and higher and higher in price with potentially no limit. So maybe it should be just another resource as done by other blockchains. And there are many different parts which can I think improved and borrowed from other resources. So I really hope that unit at the end of the day they will either change the default execution environment or that one of the execution environments in ETH 2.0 and as far, as I know, it’s expected to be more than one for different shards, that it will be brought much more friendly for zk. Or maybe let’s say just switch to a standard 64-bit integer for everything other than balances of storage and then it will eliminate a lot of pain in different places for zero-knowledge proofs too because it can make faster proofs, smaller proofs, et cetera, et cetera.

**Lucas Nuzzi:**

[1:03:40] Fascinating, and how about you, Ariel? What can you tell about the modularity of Aztec?

**Ariel Gabizon:**

[1:03:47] I can’t say much about that right now. Not in terms of confidentiality, just don’t have much on that right now.

**Lucas Nuzzi:**

You’re deeper in the weeds of the low-level primitives.

**Ariel Gabizon:**

Yeah, or at the very least I’m in different weeds. Yeah, but-

**Lucas Nuzzi:**

Absolutely.

**Ariel Gabizon:**

[1:04:12] Something I wanted to mention/plug that’s somewhat related and very interesting to me is I think we should figure out syntaxes for people, especially non-SNARK experts writing circuits that make it harder to make bad mistakes, and I’ll give a concrete example. Something you always have in, say, a Zcash style circuit is some equation saying the sum of the inputs is equal to the sum of the outputs. But of course, if you look inside the circuit, it’s usually inequality of field elements and if the quantities are too large that things start to wrap, you could get pretty bad mistakes and attacks where the output is actually much larger than the inputs. What people usually do, and what we’ve done in Aztec also is you sort of manually via range constraints and tracking things, you make sure that this wrap of the modulus is not reached.

**Ariel Gabizon:**

[1:05:35] So for example, I’m working right now in abstraction wherein our circuits for something like this, you won’t use field elements. You’ll use explicitly something called a positive integer that is some wrapper of a field element that knows to give an error like to say the circuit is bad if you reach I think the modulus. So I think that also I remember from my Zcash days, there were all kinds of cases where okay, here we really care about the bit representation. We’re not thinking about as the field elements or to explicitly think what properties you’re looking for and then to write abstractions that when people use these abstractions, it’ll be very easy that the constraints you write will be what you mean. It’ll be very hard to make mistakes like this where things are not behaving as you thought they would behave.

**Lucas Nuzzi:**

[1:06:38] Yeah, absolutely. I think that’s going to be critical for not only the overall adoption of these systems, but I think level of comfort that the community has around these systems. It’s been a fascinating conversation, extremely excited to see your projects evolve and contextualize a lot of what we discussed with actual fun implementations, and how can people find out more about your projects and get more acquainted with your work to finish things off?

**Ariel Gabizon:**

[1:07:25] Just go to aztec.network or Aztec network on Twitter I think.

**Lucas Nuzzi:**

[1:07:34] How about you, Aleks?

**Aleksandr Vlasov:**

[1:07:39] Well, yeah we have a website. [Matterlabs.io](http://matterlabs.io/), matter/labs.io. For some general overview, Twitter and Medium links and made videos of something which I talk here or basically description of the same stuff at a higher level. So yeah, it should be all found there, and if someone is interested in going actually a lower level, there is also the hiring button there. So we have a set of positions which we are always welcome to find new candidates.

**Lucas Nuzzi:**

Excellent.

**Eugene Leventhal:**

[1:08:16] Great, and I just want to thank you both for taking the time to share your work and your thoughts today. For anyone who wants to continue the conversation, please feel free to check out [smartcontractresearch.org](http://smartcontractresearch.org/) where we’re going to have a dedicated post to this specific panel which will also have more information about both Ariel’s and Aleks’s work, how to get in touch, and some information on the topic of privacy and SNARKs as a whole. So we definitely want to keep the dialogue going there beyond this conference. Thanks again, and enjoy the rest of the summit.

**Aleksandr Vlasov:**

Yeah. Thank you, everyone.

**Ariel Gabizon:**

Thanks.

**Aleksandr Vlasov:**

Yeah.

**Lucas Nuzzi:**

Goodbye guys.

**Eugene Leventhal:**

Thank you.

## Learn More About SCRF

SCRF is an interactive forum supported by an active international community. SCRF’s members work together to advance actionable blockchain research. [Learn](https://github.com/smartcontractresearchforum/docs) more about SCRF, and discover ways to [get involved](https://github.com/smartcontractresearchforum/docs/blob/main/en/content_connecting_with_scrf.md)
