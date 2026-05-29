# Leakage-under-AD-Umbrella
This is a first-order approximation check Read.Me
Threat Assumptions
Nominal raid size is 400 missiles.
Actual raid size varies according to a Gaussian distribution with 5% standard deviation. (This is so every raid is not the exact same.) Better Visuals:)
Every incoming missile is treated as an identical threat.
All incoming missiles are assumed to be successfully detected and tracked.
No decoys, penetration aids, chaff, or countermeasures are modeled.
No maneuvering re-entry vehicles are modeled.
No hypersonic glide vehicles are modeled.
No electronic warfare effects are modeled.
No sensor degradation or radar losses are modeled.
Engagement Assumptions
Defense architecture is strictly:
Aegis → THAAD → Patriot
Every missile receives the earliest available engagement opportunity.
Surviving missiles proceed to the next layer.
Layers act sequentially rather than simultaneously.
No command-and-control delays exist.
No engagement scheduling conflicts exist.
Interceptor Performance Assumptions
Aegis single-shot Pk = 0.82.
THAAD single-shot Pk = 0.87.
Patriot single-shot Pk = 0.92.
Aegis uses a two-shot doctrine.

P
Aegis
	​

=1−(1−0.82)
2
=0.9676

THAAD uses a two-shot doctrine.

P
THAAD
	​

=1−(1−0.87)
2
=0.9831

Patriot uses a one-shot doctrine.

P
Patriot
	​

=0.92

Interceptor performance is constant throughout the engagement.
No interceptor reliability degradation occurs.
No maintenance failures occur.
No launch failures occur.
Statistical Assumptions
Interceptor shots are statistically independent.

For example:

Shot 1 misses
does not affect
Shot 2 probability
Each missile engagement is independent.
Engagement outcomes are Bernoulli trials.
Monte Carlo sampling adequately approximates campaign outcomes.
Magazine Assumptions
Aegis inventory = 80 interceptors.
THAAD inventory = 60 interceptors.
Patriot inventory = 120 interceptors.
Aegis can engage at most:
80 / 2 = 40 targets
THAAD can engage at most:
60 / 2 = 30 targets
Patriot can engage at most:
120 / 1 = 120 targets
Once inventory reaches zero, that layer can no longer engage threats.
No reloads occur during the engagement.
No resupply occurs during the engagement.
Target Allocation Assumptions
Targets are allocated randomly among surviving missiles.
No prioritization occurs.
No asset-defense logic exists.
No geographic constraints exist.
No interceptor footprint limitations exist.
Any layer can theoretically engage any surviving missile if inventory remains.
Cost Assumptions
Aegis interceptor cost = $12.5 million.
THAAD interceptor cost = $15.0 million.
Patriot interceptor cost = $3.73 million.
Attacker missile cost = $1.5 million.
Cost calculations include interceptor expenditure only.
Costs exclude:
radar systems
launchers
maintenance
personnel
infrastructure
logistics
research and development
Campaign-Level Assumptions
The raid is treated as a single engagement event.
No follow-on raids occur.
No battle damage assessment occurs.
No adaptive attacker behavior occurs.
No adaptive defender behavior occurs.
Weather has no effect.
Geography has no effect.
Political constraints have no effect.
