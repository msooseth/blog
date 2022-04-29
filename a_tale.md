# A Tale of Shift Right, Frontrunning, and MEV

The NIST [Cybersecurity Framework's five Functions](https://www.nist.gov/cyberframework/online-learning/five-functions) are: Identify, Protect, Detect, Respond, and Recover. Within this framework "shift left" means that we shift our focus towards Identify and Protect, i.e. towards fixing issues before the system is deployed into production. Say, if you have a bug in your Apple Store/Google Play app, you prefer fixing it before you deploy it to the internet, or, similarily you prefer fixing the bug in your cryptocurrency contract before you deploy it in the wild (i.e. "on the mainnet"). While "shift left" makes lots of sense (let's prevent the issue in the first place!), in some sense, preventing all issues is in likely impossible.


## Shifting Left

Preventing all issues is impossible because of what [safety practicioners call](https://www.amazon.com/Field-Guide-Understanding-Human-Error/dp/1472439058) the "blunt end". When writing code, practicioners, i.e. developers, are at, what safety literature would call, the "sharp end". They are like airplane pilots, directly at the control of their craft. While it's easy to imagine that pilots are in "full control", in reality, airplane pilots depend on and are affected by many things: accurate weather reports, quality and amount of training, certification bodies, proper maintenance, production pressure from corporate, etc. These are what safety literature calls the "blunt end" -- things that contribute to both success and failure, but are not directly visible/obvious.

What this boils down to in terms of "shift left" is that while developers are in "full control", in reality, there is a large "blunt end" that they have little to no control over, and which may set the conditions up such that failure is inevitable, even with the most careful of developers. An easy example of this is previously unknown vulnerability classes: for example unknown issues with [CPU cache timing side-channels](https://www.intel.com/content/www/us/en/architecture-and-technology/side-channel-variants-1-2-3.html) in classical software, or [flash loan attacks](https://halborn.com/what-is-a-flash-loan-attack/) for cryptocurrency contracts, where an attacker can instantly obtain a large capital for a fraction of time to break assumptions about the contract, thereby e.g. helping to drain it of funds. Another obvious example would be production pressure, where competing entities are known to be working on the same idea/system and releasing first is critical for business success. It is one thing to "ask for time", it's another thing when you gotta release or it was all for nothing.

## Shifting Right

The IT security sector has realized for some time now that spending all their time on "shift left", i.e. identifing issues and preventing them, is not adequate. With some effort, time, and money being spent on detection, adequate response, and recovery, i.e. post-deployment and hence on the "right" side, the impact of attacks or unforseen events can be minimized. This is incredibly important, because as per above, it is often impossible to prevent all attacks. From phishing attacks, novel attack classes, persistent attackers, to production pressures, some attacks will go through, and be successful -- the question is simply how successful will they be, i.e. will they reach all (or any) of their intended goals, or will they be stopped early, minimizing the damage caused.

There are some interesting properties of spending proper time dealing with post-production incidents. Firstly, it allows the authors to understand what attack patterns are typical against systems. In classical IT security honeypots are 

## MEV, Frontrunning, and Shift Right




