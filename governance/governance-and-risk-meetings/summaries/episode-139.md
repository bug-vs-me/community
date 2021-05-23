# Episode 139: April 29, 2021

## Agenda

- [00:00](https://youtu.be/ZKMRegxLLXU): Introduction
- [5:50](https://youtu.be/ZKMRegxLLXU?t=350): Forum at a Glance
- [10:37](https://youtu.be/ZKMRegxLLXU?t=637): Protocol Engineering Team Update
- [22:25](https://youtu.be/ZKMRegxLLXU?t=1345): Oracle Team Updates
- [32:25](https://youtu.be/ZKMRegxLLXU?t=1945): Risk Team Update
- [38:30](https://youtu.be/ZKMRegxLLXU?t=2309): Real World Finance Update
- [43:49](https://youtu.be/ZKMRegxLLXU?t=2621): Operational Support Update
- [46:06](https://youtu.be/ZKMRegxLLXU?t=2763): MIPs Update
- [51:20](https://youtu.be/ZKMRegxLLXU?t=3080): April Governance Cycle Review
- [52:22](https://youtu.be/ZKMRegxLLXU?t=3142): Open Discussion
- [01:10:23](https://youtu.be/ZKMRegxLLXU?t=4223): Legal Team Update

## Video

<Video src="https://youtu.be/ZKMRegxLLXU" />

## Introduction

### Agenda and Preamble

#### LongForWisdom

[00:00](https://youtu.be/ZKMRegxLLXU)

- Hello everyone, and welcome to MakeDAO scientific Governance and Risk meeting #139 taking place on Thursday, April 29th at 17:00 UTC. My name is LongForWisdom, and I'm the Governance facilitator for MakerDAO.
- Feel free to interrupt. If you have comments or questions for any of those giving updates, please ask.

## Governance Update

#### Payton Rose

[01:13](https://youtu.be/ZKMRegxLLXU?t=73)

- It has been a busy Governance week. Two executives have passed our [standard weekly executive](https://vote.makerdao.com/executive/system-surplus-buffer-increase-and-burn-parameter-changes-yfi-a-addition-to-liquidations-2-0?network=mainnet#proposal-detail) that includes the system surplus buffer increase, burn parameter changes, and also YFI-A addition to Liq 2.0. Before the call, we were discussing the burner and surplus buffer. Sam will now jump in and talk about the lerp module he wrote that will go live.
  - SamM: We are using the lerp module to increase the surplus buffer. It's set to go from 30 to 60 million beginning tomorrow morning. It will take 99 days to meet the 60 million, targeting approximately 75% towards the surplus buffer and 25% toward the burner.
    - Payton: Awesome! And it's permissionless as well, which is exciting.
- The other executive that passed was our [Monthly Governance Cycle](https://vote.makerdao.com/polling/QmTxRwyh?network=mainnet#poll-detail) containing all the MIPs for the last month. Big congratulations to our four new core units being Content Production, Growth, MakerDAO Shop, and Protocol Engineering.
- We also had the [Declaration of Intent for eurDai](https://forum.makerdao.com/t/mip13c3-sp10-declaration-of-intent-eurdai/6766/17) and [MIP amendments](https://vote.makerdao.com/executive/approve-april-2021-governance-cycle?network=mainnet#proposal-detail) that passed for MIPs 4, 9, and 0. Those MIP sets added second collateral greenlight poll and allowed MIPs to be amended via the weekly cycle for their first three months of passage. Check that out if you want more detailed information.
- Concerning polls, [all four Liq 2.0 polls](https://forum.makerdao.com/t/maker-relay-ep-42/7673/1) passed. This will be moving wBTC-A and all three ETH Vaults into the Liq 2.0 framework slated for tomorrow's vote.
- Reminder: there are four days left to submit your greenlight votes on the most recent collaterals.
- Concerning Gov Alpha, we will have a meeting today with some parties interested in voting delegates. We will discuss the process and the framework. Hopefully, we'll have a detailed update on that next week.
- We are working on a GitBook Maker operation manual to assist with protocol knowledge and procedures. It is going to be helpful. We are drafting some changes to the Forum organization, so don't get too attached to the home page. We are going to be switching things around for the better.

#### Questions

- Aaron: Does the lerp module take into account the payroll deductions from the surplus buffer?
  - SamM: No. When it was crafted, we were not certain that it was going to pass.
  - Brian McMichael: Payrolls are ultimately going to be handled by the Keg, a streaming solution. The lerp is more of a point-to-point, but Keg's purpose was built for this. We'll get that out soon.
  - SamM: Coincidentally, the liquidations from yesterday completely countered the budget.
  - LongForWisdom: Yes, that's probably true.

## Weekly Updates

### Forum at a Glance

#### Payton

[5:50](https://youtu.be/ZKMRegxLLXU?t=350)

[Forum at a Glance - Forum Thread](https://forum.makerdao.com/t/forum-at-a-glance-april-23-29/7728)

##### Three-Point Summary

- “Holy liquidations Batman!” April 28th saw over \$15M of ETH effectively liquidated from ETH-B, ironically right before ETH hit an ATH.
- Liquidations revenue kick-started the burner, with over 300 MKR burned in 24 hours :fire:
- The peg remains strong, with ETH volatility likely to blame for a slight VWAP increase of DAI to \$1.002

##### Announcements

- Make sure to check out the [MIP45 Audit Summary](https://forum.makerdao.com/t/mip45-audit-summary/7612) if you haven’t had the chance yet!
- It’s the end of an era with the announcement that @Davidutro is [Retiring the Community Call](https://forum.makerdao.com/t/retiring-the-community-call/7694). It's sad. I'll leave it up to David!

#### David Utrobin

##### Community Call Farewell

[06:37](https://youtu.be/ZKMRegxLLXU?t=397)

- On Tuesday, I announced the end of the Community Call in its current form. The Community call has been the longest-running call at MakerDAO for the last few years. I've had the pleasure of hosting it. The Community Call covered weekly updates from Maker, issue discussion, special guests, and interesting technology in our space. The scope has been transformed and changed along with MakerDAO. As MakerDAO grows, we are seeing a large growth of specifically scoped community calls happening.
- I made a [forum post](https://forum.makerdao.com/t/retiring-the-community-call/7694) showing a graphic of the different types of public calls emerging. It appears to be the right time to retire the Community Call in its current form as a generalized community call. However, out of the ashes, phoenixes will rise (emphasis on the plural). I'm anticipating a lot of more tightly scoped calls. The Content Production Core Unit partnering with Growth and other Core Units will take over that Tuesday slot and do a version of the Community Call focusing on guests, BD verticals, etc. In the meantime, the Community Call is officially retired in its current form.

##### Discussions

- [Debt floor and smallholder consequences](https://forum.makerdao.com/t/debt-floor-and-smallholder-consequences/7637)
  - @jumnhy's first post to the forum asks about the state of the Debt Floor (dust) and what the community can be doing for small account holders.
- [Who do I call, if I want to call MakerDAO?](https://forum.makerdao.com/t/who-do-i-call-if-i-want-to-call-makerdao/7617)
  - @purrfection harks back to international politics and wonders how the DAO can effectively communicate with outside groups.

##### Signal Requests

- [Increase the DSR](https://forum.makerdao.com/t/signal-request-increase-the-dsr/7703)
  - @mrabino1 signals for an increase to the DAI Savings Rate, with multiple options for a “temperature check” of the community’s commitment to a positive DSR.
- [Adjust KNC-A Debt Ceiling](https://forum.makerdao.com/t/signal-request-adjust-knc-a-debt-ceiling/7706)
  - @monet-supply signals for action on KYC-A, following an announcement that KyberDAO will be moving to a new token.

### Protocol Engineering Team Update

#### Christopher Mooney

[10:37](https://youtu.be/ZKMRegxLLXU?t=637)

- It's a major accomplishment now that our team is called Protocol Engineering instead of Smart Contracts. Smart contract engineers are now moving from the foundation to a well-structured DAO. Hurrah!
- The Protocol Engineering team will be hosting office hours every Tuesday morning to make inquiries from other engineers in this space. You can also use #dev or #help on RocketChat for smaller inquiries.
- The Liq 2.0 executive is in Kovan, which includes all three Ethereum collateral types and wBTC. We're planning to put it on executive this Friday. It is big in terms of the number of assets under Liq 2.0. If there are any keepers on the call, Liquidations 2.0 is now taking liquidations. Still, we haven't seen anyone yet using the flash lending capability. There is a reference implementation of a keeper put out by the Integrations Team at the foundation. I want to encourage people to play with that and report any bugs for the two current active types, YFI, and LINK. If you manage to catch a liquidation or force liquidations yourself, and if there's a bug, please report it in #dev on RocketChat.
- The strength of Liquidations 2.0 helps us lean on Defi and single block composability to provide the liquidity to backstop the protocol without having a minimum of one keeper running on all the collateral types using that type of liquidation. We're in the same paradigm that we're with Liq 1.2, in which we need UIs or capitalized keepers to show up. It's going to be important that a keeper is running by next week.
  - Brian: I want to reiterate on the keepers. We had the big wave of liquidations the other day. Those went well with the Liq 1.0 system, and at this point, we've got a better infrastructure build-up around Liq 1.0 than we will around Liq 2.0 in the week. There are a lot of opportunities. If we have another drawdown, we're not in the same place infrastructure-wise as we're with the current system. If somebody else doesn't do it, we'll put out something for a hackathon project because we could use several different reference implementations. We would all like to have more versions of keepers that can interact with the system; ideally, we will integrate with AMMs, which will solve many problems. Still, after the Black Thursday event, we made many assumptions that 'if we build, they will come,' but that did not work. We need your help going forward.
  - Kurt: For future upgrades, the system should prioritize having more infrastructure in place and tested beyond smart contracts before rolling out to significantly large collaterals within two weeks. That is a general risk management consideration for future engineering projects.
  - Chris: There's certainly risk with staying on Liq 1.2. The liquidation process that we just had that was over 18 million USD almost filled the liquidations box with that one vault that gas liquidated. It's difficult to know the old auction systems and how well-capitalized these things will be. It's nerve-wracking at the beginning to see the bids. We were down around 12 million. We were undercapitalized by 12 million on that before the auctions were completed. There's a risk if we don't move as well.
  - Brian: On behalf of everyone from the protocol Engineering team, I want to thank the Maker community for making this transition possible.
- Chris: Regarding mandated actors, there's a multi-sig that has multiple members across multiple teams that were funded or will be funded once the monthly executive is executed. It will roughly put three months' worth of monthly operating expenses for the Protocol Engineering team into a smart contract that would be available in case of an emergency. Right now, it's funded through Dai. However, this is intended to use for emergencies. There is an entire class of emergencies concerning Dai losing value or becoming volatile. It's better to swap that Dai for non-volatile equivalent assets like USDC. If we end up in an emergency, we've at least three months of funding that will help the team clean things up or reboot the protocol and whatever is needed as long as it isn't tied to the fate of Dai.
  - Brian: Benefit of this is we will get Dai back out in the market, and it's liquid. Second, if we take on collateral types like USDC and those that go bad on this, it's unlikely that those will also go bad in the same situation that Dai does. We're trying to diversifying some of the risks through other assets.

#### Questions

- LongForWisdom: With regards to transition, do you guys have the date that you're officially free?
  - Chris: I don't have an exact date, but it's around the first week of May.
  - Brian: The Foundation hasn't told us when they are firing us. We will let you know, haha.
- LongForWisdom: Should we consider delaying big ones until we have the solid infrastructure around Liq 2.0?
  - Chris: It has been considered, and it's that risk trade-off that we just mentioned. The assessment is that with too large a pullback, the old liquidation system can't perform well. We're confident that the new system can. It requires a back stopper running. The biggest risk is that we haven't seen that backstop keeper appears in the community, and foundations can't run one.
  - LongForWisdom: That seems strange to me. Liquidation works as long as there isn't a significant pullback. Wherein for Liq 2.0, we don't know the pullback effect. It could be bad if those keepers aren't up.
  - Chris: We know that the keepers that exist can handle around 20 million in liquidations. We could anticipate that the bidding we saw with these large liquidations can also occur on a 20 million liquidation. There're some assumptions baked into it, but I think that's fine.
  - Brian: If you got the skills, assume that you know there will be a huge opportunity for cheap collateral in a major pullback. However, if everybody has the same idea, then we will liquidate you at market price. If you're on your own and nobody else has done that, you're going to get some deals.

### Oracle Team Update

#### Nik Kunkel

[22:25](https://youtu.be/ZKMRegxLLXU?t=1345)

- We're getting ready to post the Oracle Core Unit proposal. I spend most of my days now speaking with lawyers, which is not so fun. Regarding the ABDK side of things, we are already in touch with them to complete the final audit reports and announce it soon as we get that information.
- We're going to redeploy all of the existing Uniswap LP oracles to the new version that, through the help of the SC team, especially Kurt, has been optimized. It's quite efficient and will save a lot of gas fees. We want to do the rollout within the next couple of weeks. It will be dependent on how much we're trying to stuff inside the executive votes. I am not sure what the SC team planned out there, but we may have to wait until the following week if it's a bloated spell. The gas limit was raised this past week. We may have more wiggle room than we think.
- There was a [dark feed that wanted to off-board](https://forum.makerdao.com/t/7555/1). They've already shut down their feed. We need to remove their key from the oracle SC. We also need to add a Defi saver. We will work with those guys to make sure that we get those into some spells. It's a heavy operation because every time we onboard or offboard oracles, we need to get on a call with them and add or remove the feed. We currently have 15-20 oracles, which is a very heavy operation. We may perform two phases.
- Concerning Oracle R&D, we have a new pricing tool that we've been working on for an extremely long time. It's been almost a year in the final stages of testing. We want to push it out within the next few weeks. It's called `Gopher.` Currently, if you want the price of ETH-USD, you go to all the different exchanges that have ETH-USD. When you have the data, you can go through whatever data processing you want and then spit out the price. That model is inefficient because if you're querying many exchanges, some of the APIs don't respond in time, and others may time out. A better way would be to ping exchanges for all the data and prices constantly. You will have all of those prices cached. When you want to know the price, let's say ETH-USD, you now have all the data for signal processing.
- In parallel, we've another new feature that we call `Spire,` which enables another P2P solution to back up the Oracle system. Many of you might be aware that we had issues with Scuttlebutt within the past year, particularly thanksgiving. Scuttlebutt is a P2P network where all of the feeds are exchanging price messages.
- Regarding the Oracle Stack, we want to make sure that everything is hyper resilient. If any of the components breaks, such as pricing tools, then there is a backup pricing tool. If this networking layer breaks, then there is another networking layer. Hence, with `Spire,` we will have Lib P2P acting in parallel with Scuttlebutt. If Lib P2P fails, we have Scuttlebutt and vice-versa. The next step would be to get the client diversity, just like ETH 2.0 has multiple clients; We have Teku, Nimbus, Prism, and Lighthouse. We want to have multiple reference implementations that follow the same common spec. Right now, we have one oracle client, `Omnia.` We are beginning to create a second reference implementation called `Ghost.` after that, I would like to see a third-party team as part of the core unit to give some money in helping to create different client and maintain them. This diversification helps us to stay away from repeating the same design approach.

### Risk Team Update

#### Primoz Kordez

[32:25](https://youtu.be/ZKMRegxLLXU?t=1945)

- We are preparing to release the next batch of proposed parameters for Liquidations 2.0 for the remaining vault types. We will propose parameters for the ten smaller vault types. We will cover them this week, and next week, we'll propose some parameters for Uni LPs. According to the plan, we have all vault types activated apart from stable coins and PSM in Liquidations 2.0. It should take less than three weeks but depends on the voting process and the Smart Contracts team to implement everything according to the plan.
- As was mentioned today, @Monet-supply made a [signal to lower the KMC debt ceiling to zero](https://forum.makerdao.com/t/signal-request-adjust-knc-a-debt-ceiling/7706) because the KMC token is being migrated to a new version. We need to disable the vault. There are a few methods to do that. We will likely propose to decrease the DC. We can gradually increase the stability fee, and at some point, we will probably disable Oracles. We will then see whether the new KMC token will be onboarded soon after because this was the lowest utilized vault. We have seen 10,000 debt exposure on average in the past, and this vault costs Maker more than it was earning through the stability fees.
- We started preparing for a new set of collaterals evaluations. There was a consensus between other facilitators that the future focus will be on Sushi LPs. A few applications for Sushi LPs were already [posted](https://forum.makerdao.com/c/collateral-onboarding/co/17) this week, and we will likely soon choose between those pairs to begin working on evaluations.
- Yesterday, we had an analysis on ETH-B auctions. Surprisingly, the bids were solid this time. This surpassed expectations because ETH-B auctions haven't been perfect in the past. I'm going to mention a few metrics; There were about 360 auctions in total. The total amount of debt liquidated was 16 million, penalty fees collected 2 million, which is a full collection of penalty fees. There were only 16 auctions where a fraction of penalty fees were not collected. Maker could collect another 20 thousand more Dai. There were between two to three addresses that were bidding, which is more than usual. There were also two-thirds of initial bids or zero bids, something that was observed in the past. The good news is that Liq 2.0 will make zero bids impossible. From the Maker side, the outcome was great. We saw a good response. We also confirmed the `box.` The pending liquidation size limit isn't too high. Keepers were fairly capitalized. the most significant metric is the profit keepers made or how much the vault owners lost. This number was good considering the best results because auctions settled on average at 4% below market price. This means that vault owners lost penalty fees and another 4%.
- We had surplus auctions, the so-called `flap` auctions. We hit the 30 million surplus. They are doing fine. MKR being sold in these auctions is on average 5% above market prices. There isn't a large number of keepers bidding in these auctions. On the other hand, we won't be seeing this huge amount of `flaps` anymore because we are increasing the surplus buffer unless we have a larger liquidation event again.
- Besides the ongoing release of Liq 2.0 parameters, we are also working on updating risk parameters. Usually, on our side, at the end of the month, we update three premiums DCs, which are then used for the parameter proposal group that meets next week. We expect to have new suggested parameters for May.

### Real-World Finance Team Update

#### Sebastien Derivaux

[38:30](https://youtu.be/ZKMRegxLLXU?t=2309)

- Update on NewSilver: More loan audits were made last week, and now we have half a million invested in this NewSilver vault.
- We have a call with the legal team next week to discuss monthly due diligence and concentration in Florida. Initially, we made the limit of 30% in maximum exposure of any state in the US, but there's been a lot of activity in Florida. We will ask him about stopping low-exposure loans in Florida if the threshold is met. Otherwise, everything is working fine. There was also the new drop of investors in the pool, making repayment of Maker loan. That's why it's 400k; we can know that all the smart contracts are working from this.
- Regarding collateral onboarding, we will try to push a new batch of Centrifuge assets either the end of next month or the first week of June to be ready on our side and evaluate up to 4 Centrifuge assets. We will be able to onboard whatever Governance decides.
- We made progress on trust models as well. Matthew [released new documents](https://forum.makerdao.com/t/rwa001-a-custody-agreement/7724) today. we're still confused about its success as well as the other ones.
- I had a call with a lawyer yesterday. A month ago, it was the first call with Arnold & Porter LLP. We had a call with a partner in the US who's an expert in structure finance, and he has some connections with Arnold & Porter. They also lobbied for crypto in Washington. They have good expertise in regulation as well. I will write documentation about MakerDAO and the regular assets for MakerDAO to help them get up to speed. If everything works, we will begin to hire them next month to audit NewSilver investments.
- Finally, we surpassed 10 million in monthly revenue, which is an all-time high. I will present the monthly financial reports early next week, and maybe we will be able to discuss them in the next G&R call.
  - David: How much revenue we made from PSM this month?
  - Seb: I don't have a hard number, but I saw they were below 1 million, which is relatively insignificant for Maker.

### Operational Support Update

#### Juan Guillén

[43:49](https://youtu.be/ZKMRegxLLXU?t=2621)

- We have been busy transitioning to SES and incorporating a lot of feedback that's been given to us. Amy is working in the background on various projects in the foundation.
- Regarding Know Your MIP, we had Stani from Aave and some presenting [KYM #8](https://forum.makerdao.com/t/know-your-mip-kym-08-mip50-direct-deposit-module-monday-april-26th-17-00-utc/7566/3). MIP50 was very interesting. The recording is on YouTube.
- Yesterday, we had [MCO2](https://forum.makerdao.com/t/collateral-onboarding-call-31-mco2-token-wednesday-april-28-16-00-utc/7615), a carbon credit market application, the MIP6 application that is already on YouTube.
- On the core units side of things, we had [Request Network last Friday](https://www.youtube.com/watch?v=9nwTPJo3d50) explaining how to use it and showing their new features. Tomorrow, we will have a [workshop to set up OKRs](https://forum.makerdao.com/t/core-unit-rituals-01-okrs-workshop-with-andy/7682) with Andy from SCS.

### MIPs Update

#### David Utrobin

[46:06](https://youtu.be/ZKMRegxLLXU?t=2763)

![](https://i.imgur.com/iKL6ZuL.png)

![](https://i.imgur.com/RZiiYgN.png)

![](https://i.imgur.com/7CtbfHD.png)

![](https://i.imgur.com/eoYc7vh.png)

![](https://i.imgur.com/90n3Cpa.png)

![](https://i.imgur.com/GWoXvUR.png)

![](https://i.imgur.com/RsXiY05.png)

![](https://i.imgur.com/OmQQP4g.png)

![](https://i.imgur.com/KULr1Nl.png)

## Procedural

### April Governance Cycle Review

#### LongForWisdom

[51:20](https://youtu.be/ZKMRegxLLXU?t=3080)

- We managed to avoid the issues we had with MKR voters this month, at least for the MIPs. We had trouble getting things passed in time for the executive on Monday. It worked out in the end, but it's good to highlight this situation. This is the main reason why we are proposing the change to the Monthly Governance cycle, which David referred to as [MIP51](https://forum.makerdao.com/t/mip51-monthly-governance-cycle/7366). Hopefully, that will help resolve the issue in the future. It includes changes to the way that the monthly event cycle works. We may take time next month to discuss it when it goes into voting.

## Open Discussion

[52:22](https://youtu.be/ZKMRegxLLXU?t=3142)

### Governance Core Cycle

- LongForWisdom: This is the moment for everyone to present comments or questions regarding the last monthly cycle. Chris Mooney states that he is in support of the change. It should change the Governance cycle slightly and make things easier around executives. I encourage everyone to read over MIP51 to have an understanding of how things are changing. Also, we saw a lot of new Core Units get ratified. We offer congratulations to those facilitators and those within those Core Units that went through. It's been fantastic to see more people joining the DAO.

### MKR compensation working group

- David Utrobin: I am curious whether there is an update concerning the MKR compensation working group? We have to discuss all these queries coming to fruition.
  - LongForWisdom: I haven't mentioned it up to this point because the group was not yet ready to publicly state anything definitive. We met last Friday, and we've been meeting every day since then to discuss various things. We are making progress. We continue leaning towards guidelines and strict restrictions. The hope is to lay out some guidelines, Core Units that are less sure about MKR compensation. Also, guidelines that allow Governance to compare individual core units' compensation structures against the guidelines that we put initially release. We set a rough target for May 10th to have something substantial and formal released for everyone. In the meantime, we will continue to work on it.
  - Payton: We approved protocol engineering testing. They've got some contracts working, but will there be further discussion on that structure, or will that be included in an upcoming executive?
  - Derek: Are you referring to the mechanism or the quantity?
  - Payton: The mechanism has already been approved in terms of minting or how it's done.
  - Derek: Perfect. Brian has written a contract called DssVest. We have a specification written up for it. I imagine us submitting it to the forum within the next few weeks. I want to keep the focus on Liq 2.0 for the time being. Nonetheless, it's written up and will be posted as soon as we get past this hurdle of Liquidations.

### Governance and Risk Meeting Structure Discussion

- LongForWisdom: Does the structure of this meeting meet the audience's requirements? Could it be more effective, and how well would it scale as we add more Core Units? Some people state that they like it the way it is. Other people would like to see some changes. Does anybody want to chime in?
  - Chris Mooney: I tried to change the format of the Protocol Engineering team meeting disclosure. I was doing stand-up with the entire DAO, and we had to surface the important stuff at some point. I like the format of this meeting. I think it's necessary. It's going to have to change shape, and it's funny that it's "Governance and Risk" because we are a little off that mandate. It's more like an all-hands.
  - LongForWisdom: Yes, that's fair. I have this bad habit of assuming everything is Governance because it all involves Governance knowing things.
  - Kurt: I was going to make that exact point. All decision-making for the DAO falls under Governance.
- Aaron (in the chat): When will Growth have a section in this meeting?
  - LongForWisdom: Probably next week. I haven't yet spoken with anybody from the new Core Units. They are all welcome to do a weekly update. I encourage you to get in touch with me to slot a regular segment. I hope we will begin to see biweekly updates.
- David Utrobin: This call is primarily focused on updates and issue discussion. Eventually, updates will continue to grow. The benefit of having the "issue discussion" as part of this call is that everyone is present; it's an all-hands event, and you have all of the key people ready to give feedback. If we were to split off the Governance and Risk meeting in the future, my recommendation would be to do a town hall for updates and a town hall for issue discussion. Make sure that people attend both at similar levels of importance. My main concern is with this call becoming way too bloated through the growth of Core Units and issues, etc.
  - LongForWisdom: The issue discussion concern is important. As you say, it's a chance for people to discuss whatever they want with all the involved people. I haven't explicitly considered splitting up, but we could potentially do something like that. We could publically split up this meeting and follow an agenda of the first 45 minutes for updates, and at the end, we initiate the discussion. Anybody can show up to both calls.
  - David Utrobin: Yes, I like that idea a lot.
  - LongForWisdom: Five-hour-long calls are a shock. I want to avoid adding time to this meeting. I know a lot of people find this useful. Some people are already frustrated by its length. It's one and a half hours long on a regular. I wouldn't want to push far above that. @juanjuan, I know you had some comments on the meeting. Do you have anything to share?
  - Juan Guillén: I'm a little more empathetic. I want to make sure that we don't talk to only each other and that we are more inclusive. I'm thinking about the objective of this call; what the audience wants and why. I asked many questions to several people. I would like to know if the people who see this once a week believe that's enough for them? What was the objective of the call: more to discuss things, give updates? That's the road I went down. Unfortunately, I don't have a solution. I would like to hear any ideas and opinions.
  - David Utrobin: Regarding the discussion section, one of our disadvantages is that we don't plan very deeply for what we will discuss. Generally, it works out. But it is critical to know who the relevant people are to discuss certain issues and make sure they are available and present for when those issues are discussed. If we do split off into more focused "issue discussion calls," inclusivity is a huge deal by being able to have everybody there and synced. It's very important to have that.
- LongForWisdom: We often run these calls, and we have fairly full audiences, right? But it tends to be the same people speaking, those that are most familiar. If you are someone in these calls which doesn't often speak, and there's anything you want to share with me privately that you think we could do to make it easier, please feel free to speak right now.
  - Kurt: It's important to not get in the habit of making decisions on this call. Any call will not line up well with at least one participant's time zone, And people may have other reasons they can't make a call. It's important to emphasize the more asynchronous forms of communication for finalizing decisions, namely the Forum and RocketChat, for more ephemeral things.
  - LongForWisdom: That's another good point. That's always been the goal, to avoid actual decision-making in these calls. Generally, we do fairly well with that. We often have people proposing courses of action, but we don't determine them, not in the regular call. However, there are some emergency examples that we had.
  - Kurt: Many contexts come through in this call. Now that we have the great summaries, people can catch up on them and review the discussions. Thereby, they can raise it in a separate forum post. Even though we don't explicitly make decisions, sometimes the context of this call carries through to what the decision will be. It's important to make sure that it gets out there and everyone has a chance to respond.
- Payton: Would an anonymous question line help make sure we can get people to answer without necessarily putting them on the spot in front of everyone?
  - LongForWisdom: Yes, that's a good idea, especially for those who watch the call but don't tend to show up live. We could put something like that together.
  - Christopher Mooney: Yes, that's a really good idea. I've seen this done in larger companies, but it also works in our community because people want to maintain their anonymity.
- Matthew Rabinowitz: Another idea would be the mandated actors who go through the normal cycle. In many ways, so much of what is being said on those calls could be pre-recorded and put on YouTube or somewhere else as a reference. People could watch them in advance. Those who don't watch it could hear the top three salient points of that video. This would allow us to get through an entire section much faster where there are all the references elsewhere.
  - Kurt: Any reasons why you suggest video segments as opposed to a text-based format?
  - Matthew Robinowitz: Either way. Some people prefer to talk. Others prefer to type.
  - LongForWisdom: We considered that before, and the concern I have is that it requires more coordination for anyone that wants to keep up to date. With the current setup, the call is during a fixed time; we show up, and then that's all good. If it becomes meaningful to participate, I need to read this document, watch these videos, and show up. But maybe that's something the people and community could perhaps do or would even want to do. Payton has good experience with speeding up meetings, but it may be difficult to enforce it on other people. We can always try.

### Legal Team Update

#### Matthew Rabinowitz

[01:10:23](https://youtu.be/ZKMRegxLLXU?t=4223)

- We worked with Chris through the MIP21 circuit and confirmed that the RWA001A moved 50 Dai back and forth.
- Yesterday, we had a two-hour conference call with WFSF Bank. We went through the entire structure, and they are ready to go. We somewhat of a "chicken in the egg" scenario; the custody account needed to act as a bank account needs to be formed to connect with the broker-dealer. You can't have that until you the trust is formed. We don't have the trust formed yet because the community hasn't greenlighted the transaction. We will perform an interim step; we will use a short form trust agreement that intentionally shortens it. This will be amended and restated by the actual operative document that we'll be putting in the forum in short order. That will allow us to form the account to connect it to the broker-dealer and short-circuit in a couple of weeks. We went through the trust agreement comments that we put forth. I wouldn't say they push back. They have some concerns, but they are integrating them.
- ![](https://i.imgur.com/0a8W6it.png)
- This is an exhibit that has not yet been accepted.t this is the general narrative of what we're trying to advance and into the trust agreement. The entire trust structure includes all the legal documents, credit agreements, and downstream documents. There are hundreds and hundreds of pages that very few people will read. Frankly, the trustee, the LendCo, the trust sponsor are the parties that need to be involved in every line. And they are. The most important idea to grasp is the narrative that we are trying to mimic, what we use with crypto vaults but in a real-world structure. In the context of being a verification agent, the trustee will be responsible for funds that come in and come out before they can issue a loan. Once a loan is repaid, they need to verify the outstanding debt for this given vault and then compare it to the DC. If one is greater than the other, then there's a certain action they have to take, which cuts off the downstream credit and allows the downstream loans from that to unwind organically. It's no different if we took the DC on ETH-A, when it's outstanding at whatever it is, 2 billion, and change it to 1 billion. None of those loans would be foreclosed upon or be liquidated. They would sit there while people would complain that they can't take out new loans.
- The context is the same with the DAO's ability to issue a liquidation order to trigger the liquidation event that the trustee will monitor and check on a routine basis to see if the DAO has initiated that. I always want to stress that this is a nuclear event and, as I [posted in the forum](https://forum.makerdao.com/t/6s-rwa001-a-how-makerdao-is-protected/7723) earlier today, how MakerDAO is protected in this context. The LendCos have certain covenants pursuant to the credit agreement. If they don't meet those requirements, the trustee will be the party that will liquidate LendCo faster than the DAO ever will.
- We spent some time yesterday working through the verification process. This is an essential point for every trustee that is ever going to be a trustee for what this type of structure will be used. It's going through the educational process of learning how to read it at a core level. It doesn't involve cool UI and UX - I like Dai Stats and Maker burn; it's all neat but, if somebody was nefarious, how much of that could be manipulated? We have to make the game theory for how we get the trustee to read the blockchain. Fancy UX portals are neat, but how do they go down the next layer? I sent out a forum post, and Chris went through it and confirmed the sequences. I have a verification portal that I'll be using with WSFS Bank. It's currently in the early alpha stage. the imperative point would be that they need to learn how to affect Etherscan. This is marrying two worlds that never were destined to date. How do you have a trustee that's spectacular with paperwork and perfected UCC1 senior position loans as well as looks at blockchain and the numbers?
- We do have a step sequence portal that's largely automated. We would feel on their perspective. It's like being a pig on roller skates; 'You want me to do what? I click on this contract, and it says `ilk,` what does that mean?' We can all smile at it, but it's true. Eventually, they'll realize it is not a big deal and turn into the routine course of business.
- That is all I have to cover right now. We are in the final stages. I posted the [custody agreements](https://forum.makerdao.com/t/rwa001-a-custody-agreement/7724/8). We were patenting the security agreement, which is a UCC1 document. It's very straightforward. After that, we have the credit agreement, which is 60 pages, followed by the trust agreement. These two last documents contain all the salient points. The community needs to compare them to the term sheet presented. Some minor changes are lightly in favor of the DAO. None of the changes were against it or in favor of me. one major change is the addition of another tenant, which was already outlined in the downstream documents, including Tesla.

##### Further Discussion

- [Someone](https://youtu.be/ZKMRegxLLXU?t=4673): Our RWA Core Unit has attorneys looking at this. Have they given back any input to the community?
  - Sébastien Derivaux: Yes. We are in discussion with Arnold & Porter LLP. We are waiting for the final document from Matthew. We will use them first on the assessment of NewSilver. We will also have those lawyers review this structure. It might take some time, and we could first look at the structure ourselves. We have a good lawyer, Christian, in the community. He might help with that. He is used to those structures. We need to find a good strategy between acting fast, being bulletproof, or 100% confident. First, we need to be sure that it's working. If minor details need to be fixed later, it's less of a big deal. For instance, I checked some documents, but I thought that Cayman Entity has ownership of the funds, and the funds are transferred in US dollars in them, no longer in the Delaware trust. It's the initial MIP. I saw that Martin is now director or at least has executive power in the Cayman's Entity. It seems to be a trustee of the Delaware trust as well. That's what we need to figure out.
  - Frank Cruz: It was going to be Dai that went into Cayman, right?
  - Sébastien Derivaux: Dai would go to the OTC broker, but then the broker would send the funds to the Delaware trust instead of the Cayman Entity. Cayman Entity was the owner of a smart contract but unable to do anything. This was why they couldn't prove that they were the owners of the wallet.
- Matthew Robinowitz: The way this structure is contemplated is that there is a trust sponsor, which is the party that creates or causes the creation of a Delaware statutory trust. In this case, it is a Cayman exempt entity. It becomes in possession of Dai and automates by the smart contract to sends that Dai. There is a gap where it becomes legal in a "term to rest." Dai is sent, bumped, or pushed to the broker-dealer, which will have irrevocable transfer instructions to immediately exchange that dive for US dollars and send them to the Cayman Entities account at WFSF Bank. That account then has irrevocable transfer instructions pursuant to that escrow agreement to transfer those US dollars to the trust that is now underneath and governed by that trust agreement. It's exactly the reverse whenever funds are returned.
  - Sébastien Derivaux: Yes, the irrevocable transfer on the bank account is something that I don't know is possible and how irrevocable it is.
  - LongForWisdom: These are questions for another meeting. Thank you for the update, and it's good to see progress made. I will talk to you all soon!

## Common Abbreviated Terms

`CR`: Collateralization Ratio

`DC`: Debt Ceiling

`ES`: Emergency Shutdown

`GF`: Governance Facilitator

`SF`: Stability Fee

`DSR`: Dai Savings Rate

`MIP`: Maker Improvement Proposal

`OSM`: Oracle Security Module

`LR`: Liquidation Ratio

`RWA`: Real-World Asset

`RWF`: Real-World Finance

`SC`: Smart Contracts

`Liq`: Liquidations

## Credits

- Artem Gordon produced this summary.
- David Utrobin produced this summary.
- Gala Guillén produced this summary.
- Sai Teja produced this summary.
- Everyone who spoke and presented on the call, listed in the headers.