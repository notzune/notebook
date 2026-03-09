 #ACR

# Main goal

the main goal is to implement a more complex and intuitive economy system that incentivizes commerce. the plan is to design a system where merchant gameplay is viable. we can try and eliminate some of the harder aspects of actual trade based economy and instead make it easy to earn passive income in the form of NPC stand-ins while still adding gameplay mechanics that build on to the immersion of being a business tycoon. 
## Currency system

the economy system will implement a "physical" (item-based) currency. the currency object can be structured so that each item has a UUID that can be checked against a cache of UUIDs to ensure that a currency is "minted".

ideally I want to design a system where nations can mint their own unique currencies with an exchange rate.

the issue is figuring out what the value of the currency would be tied to. the obvious answer would be stock of precious metals such as gold. 