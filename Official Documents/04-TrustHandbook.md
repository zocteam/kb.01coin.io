/*
Title: Chain of Trust Handbook
Sort: 4
ShowOnHome: true
*/

![](https://github.com/deadthings/kb.01coin.io/raw/contrib/Official%20Documents/TrustHandbook01.png)

By: deadthings
Date: May 30, 2018

# Background

The Chain of Trust is a computer security concept that stems from certificate authority (CA). It is a method for validating each component of hardware and software from the end entity up to the root certificate. It is designed to ensure only trusted hardware and software can be used while still maintaining flexibility.

Any item of hardware or software only needs CA keys that are trusted by the parent hardware or software with which it interfaces. So long as that parent item is trusted by its predecessors sequentially, all the way up to the root certificate, then trust in the new item of hardware or software can be assumed by the root certificate due to the Chain of Trust.

Utilizing this Chain of Trust construct as a method for developing trust within a community and fostering good project stewardship among members of that community was first theorized by 01coin lead developer OwenRay in his 01coin Takeover and Change Proposal originally published on March 22, 2018. 

In that document, OwenRay wrote,

> *"In business people have to work together all the time. There is a certain amount of trust needed to do this effectively. While you may wish to be able to trust co-workers or employees to be “perfect,” you must be wary of intentional or unintentional mistakes. That’s why you build trust and give power over time. But whatever you do, you always have a safety net (backups, version control, etc.).*
> 
> *"For 01coin this means as community members prove their value to the project they will be assigned more and more important roles. But there should always be safeguards. No-one should be able to take destructive, non-reversible actions. At a certain point people should also be trusted to trust. This means you allow members to assign roles themselves. It’s like saying, “Because I trust you, I trust who you trust.” This way you’ll create a “Chain of Trust” similar to that used in computer security certificate authority (CA).*
> 
> *"The trust and empowerment members will receive does not only apply to Discord or being able to participate in advanced governance structures, or invitations to review code. It has to apply to every product 01coin will produce. From whitepapers to websites to development projects, the community should be in control."*
 
# Your Responsibilities as a Chain of Trust Member

Being a trusted member of the 01coin community is a privilege that comes with a degree of responsibility. Chain of Trust members are expected to exercise good stewardship of the project at all times. That means acting with integrity and putting the best interests of the project ahead of your own person self-interest, although in most cases the two will be intertwined. 

As a member of the Chain of Trust, you will have the authority to either add new members or promote existing members to lower levels on the trust chain, as well as nominate promotions for other members to your own trust level. In so doing, you are expected to act with care and diligence. Make sure you scrutinize your choices closely and have a clear rationale for your actions. 

As a general guideline, it is expected that a community member will have to make meaningful contributions to the project over a period of time before being awarded a Chain of Trust role. As the blockchain already awards contributions for mining and masternode ownership, the contributions of interest to the Chain of Trust may include coding, tech support, marketing, etc. And that member should continue to put in those efforts over time at each successive level they reach on the Chain of Trust in order to be considered for promotion. 

It should be noted that the Chain of Trust is – for now at least – being administered solely on the Discord server. In reality, though, this trust extends to individual members across all aspects of the 01coin network including social media, governance, development and perhaps eventually the blockchain itself (although there are as-of-yet unanswered questions regarding the maintenance of privacy and anonymity in attempting to implement this).

# How the Chain of Trust Works

A Trust LVL1 member has the following authority: They may nominate an as-of-yet untrusted member of the community to be awarded a Trust LVL3 role. This nomination will be subject to debate among Trust LVL2, Trust LVL3 and zocteam members until a conclusion is reached whether to accept or deny the nomination.

A Trust LVL2 member has the following authority: They may award a Trust LVL1 role to an as-of-yet untrusted member of the community AND they may nominate a Trust LVL1 member to be awarded a Trust LVL2 role. This nomination will be subject to debate among Trust LVL3 and zocteam members until a conclusion is reached whether to accept or deny the nomination.

A Trust LVL3 member has the following authority: They may award a Trust LVL1 role to an as-of-yet untrusted member of the community AND they may award a Trust LVL2 role to a Trust LVL1 member AND they may nominate a Trust LVL2 member to be awarded a Trust LVL3 role. This nomination will be subject to debate among zocteam members until a conclusion is reached whether to accept or deny the nomination.

Trust LVL3 members also have the additional authority to nominate proposals to be considered for future 01coin development. They may participate in debate over these proposals and, alongside the zocteam, vote on which proposals are added to the 01coin network governance infrastructure for the final vote, which will be carried out in a representative fashion by the entire 01coin network as a whole. Lastly, the Trust LVL3 members will be the first considered when there is an opening on the zocteam.

The principles of the Chain of Trust are also being exercised by the zocteam on our GitHub account on a smaller scale. Access and permissions are progressively earned.

In CA, when a top-level trust agent loses trust, all of its downchain agents are doomed to lose the root certificate’s trust as well. This is where the social implementation of the Chain of Trust deviates from CA. When a member of the Chain of Trust takes action in a way that could be interpreted as inconsistent with their responsibilities as a Chain of Trust member as articulated above, upchain members will discuss the implications. If it is decided that this action is indeed counter to the values and purpose of the Chain of Trust, the offending member will lose all trust. Note this does not result in a downgrade of trust level, but rather a full revocation of trust. That member’s own downstream Chain of Trust members will not be impacted and will retain their existing level of trust.

# Conclusions

By implementing the Chain of Trust, 01coin hopes to not only build a strong community around 01coin, but also one that exercises industry-leading stewardship over the project. It is in 01coin’s best interest that a large and representative cohort within the community are able to take on greater and greater leadership roles as time goes by and as the project matures. Through this mechanism, and the future network governance infrastructure yet to be implemented, we hope to achieve our goal of making 01coin the benchmark blockchain project for community governance in all of crypto.
