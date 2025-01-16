## Goals

### Accuracy

> Once the room temperature stabilizes, what's the maximum temperature difference in $\pm1^{\circ}\text{C}$ I can expect from what I set?

The system tries to keep the temperature within $\pm1^{\circ}\text{C}$ of what you set it to.

If your AC has $1^{\circ}\text{C}$ temperature steps, there is a theoretical minimum error of $\pm0.5^{\circ}\text{C}$ when your ideal temperature falls between two steps. Plus, temperature sensors aren't perfect.

### Latency

> Are you trying to cut down on those beeping sounds from sending too many AC commands?

Nope! I'm letting the system fire off as many commands as it needs to get the temperature right quickly. If the beeping bothers you, you've got options:

- See if your AC has a setting to turn off those beeps

- Pop in some earplugs while you sleep

> Are you keeping the fan speed low to make it quieter?

No. I'm letting it run at whatever speed gets you to the right temperature fastest. If the breeze bothers you, you've got options:

- Point the AC away from your bed and you won't feel the air hitting you

- Earplugs are your friend for a good night's sleep anyway

### Consistency

> How long is `config` designed to run once it's set up?

Once set up, `config` aims to run for at least a year without any extra tinkering.

> Do I need to press any button before bed?

Nope! The schedule automatically kicks in and finishes up based on the times you configure.

> Will the schedule adjust if I go to bed earlier or later than usual?

No. `config` doesn't track your actual bedtime. It only follows the times you've configured.

If you turn in early, you'll still wake up at the usual time.

And if you stay up late, you'll likely feel a bit more tired, which encourages you to head to bed earlier the following night, keeping that sleep schedule nice and steady over the long run.

### Budget

> What's the maximum budget for setting up `config`?

The plan is to keep the total cost under $1,000, significantly less than high-end smart beds that can easily run into the thousands.

### Minimalism

> Which does `config` prioritize more: a smaller hardware footprint or a simpler setup process?

`config` places a higher priority on reducing the hardware footprint. Setting things up only happens once, but extra devices clutter your space every day.
