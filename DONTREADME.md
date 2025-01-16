## Goals

### Accuracy

> Does air temperature affect sleep onset latency (SOL)?

Oh yeah, definitely! This study showed SOL is significantly shorter when the room is at $26^{\circ}\text{C}$ compared to $23^{\circ}\text{C}$ or $30^{\circ}\text{C}$ (https://www.sciencedirect.com/science/article/abs/pii/S0360132313003442#:~:text=The%20duration%20of%20sleep%20onset%20latency%20(SOL)%20was%20longer%2C%20the%20duration%20of%20slow%20wave%20sleep%20(SWS)%20was%20lower%2C%20and%20the%20subjective%20sleep%20quality%20was%20lower%20at%2023%C2%A0%C2%B0C%20or%2030%C2%A0%C2%B0C%20compared%20with%2026%C2%A0%C2%B0C.).

Some folks might dismiss this as just p-hacking, but I've got a foolproof way to prove air temperature affects SOL. Just try sleeping at 26K. You'll rest in peace! 😉

> Is the target temperature based on skin temperature measurements?

Nope, it's not! Using skin temperature can be unreliable for a few reasons:

- Movement: Skin temperature sensors can shift around while you're asleep, which messes with the readings.

- Blanket: If you're wearing the sensor on your wrist, arm, or finger, it might sometimes be under the blanket and other times not. That can make the temperature readings jump around, depending on whether it's covered or exposed.

> Is the target temperature based on the temperature reading from the AC unit?

No. The target temperature isn't based on the temperature reading from the AC unit. The goal is to hit the target temperature the bedside sensor is reading, not the AC unit itself.

The problem is, the temperature near the AC unit is usually higher than what you feel at the bedside. There's this thing called temperature stratification, where the air can be several degrees warmer near the ceiling than near the floor sometimes by as much as $5^{\circ}\text{C}$ (https://www.sciencedirect.com/science/article/abs/pii/S037877881100274X#:~:text=even%20for%20a%20relatively%20small%20height%20of%20the%20enclosure%2C%20a%20temperature%20difference%20of%20about%205%C2%A0%C2%B0C%20exists%20on%20the%20vertical%20direction).

Subtracting a constant amount from the AC's reading might seem like a solution, but it's not that simple. The temperature difference depends on things like:

- The temperature of the walls, floor, and ceiling

- The settings of the heating or cooling system

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
