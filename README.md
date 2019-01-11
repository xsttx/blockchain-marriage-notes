# blockchain-marriage-notes

My comment from a Facebook thread (slightly modified for context and clarity) reposted here, to invite to public debate on the subject:

# BLOCKCHAIN MARRIAGE CONTRACT DESIGN

This is how I think the ideal marriage contract should be structured:

The foundation of the contract code should be a multisignature wallet. This permits you to manage funds and tokenized mutual assets together. Tokenized assets can be anything from vehicles to furniture, or stocks and bonds, whatever. A good multisig can also own and manage other contracts (like a child care contract, a will, a land title, etc). The Gnosis multisig wallet, or rather a modified version of it, could be used for that purpose. Since it's a multisig, you can also add people in (like children, for instance) when needed.

Challenges with that approach:

1. Roles - there should be a possibility to add different roles. For instance, you wouldn't want a 5 year old child to have the same tx signature permissions as an adult parent, for obvious reasons. This would also allow to add things like witnesses, arbitrator, or a family priest or lawyer or whatever people deem important to their union.

It can easily be solved with weighted signatures, but the issue is that, as far as I'm aware, there's no multisig who does this efficiently yet - hence the code would have to be throughly audited, which is expensive (it has to be a high quality 3rd party auditor since people will hold funds in the wallet).

2. Identity - ideally you would want to be able to verify the identity of those who signed, to avoid people claiming things like "look I'm married to this person, it's on the chain" while in fact it was not at all the person they claim it to be who signed the contract.

This can obviously be resolved with signing off on it with a public key, like we have on the Bitnation jurisdiction (could include a possibility to add something like a nation state issued ID, for those who wish to do so), or it could be done more "hacker style" i.e. during a live meetup with witnesses who signs of with their pgp key on a photo with the couple, latest blocknumber and so on.

3. Divorce - assuming the contract has weighted signatures, one of the parties can choose to remove their signature permission or their partners, if the other persons signs of on it. Let's say it's a union of two individuals, they each have 10 signatures in their signature, and the total needed is 15 out of 20. It means that if they want a divorce, if they and 5 other people who's signature is worth 1 for instance (could be worth more for someone like a mutual child), then it works. The only issue is if the person want to remove the other person, while they have mutual assets in the contract, through a collision. I guess there could be some sort of solution like the two main parties need to sign of on it themselves to remove themselves, but I have no idea what that would look like in code form or if it's even doable.

--------

In addition, a non-programmable document with guiding principles/ ethics (on things like fidelity, plans, wishes) can be referenced in the multisig wallet code, to be used as a reference in case of conflict and arbitration. The non-programmable contract could also refer to a code of law, like Civil Law or Common Law or Sharia or whatever, to be used in case of disputes. Basically a "marriage declaration" or a "marriage constitution".

The multisig approach also means that only the things that you both choose to put in the multisig contract (funds, assets, other contracts) are shared, the rest is privately owned by the individuals, per default.

I haven't seen anyone take this approach to a marriage contract yet, but it seems to me like the simplest solution which offers the most functionalities.
