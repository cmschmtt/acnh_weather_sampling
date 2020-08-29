# ACNH Weather Sampling Strategy for Identifying Weather Seed

I wanted to use MeteoNook to identify my Animal Crossing: New Horizons weather seed, and my initial approach (time traveling to check the weather at random hours until the website told me I had enough information) seemed inefficient. With data from the [MeteoNook repo](https://github.com/Treeki/MeteoNook) repo ([website](https://wuffs.org/acnh/weather/)), I settled on this method of checking weather:

- Check the weather at 7am/7:00 and enter it.
- Check the weather at 1pm/13:00 and enter it.

This alone is sufficient to identify 12 out of 17 weather patterns. The 5 remaining weather patterns are sunny at 7am and sunny at 1pm.

If 7am and 1pm are both sunny,

- Check the weather at 3pm/15:00.
- If it is still sunny at 3pm, check the weather at 4pm/16:00.

### A few disclaimers

- I assumed each weather pattern was equally likely; this may not be the case.
- This is of course fastest if you are willing to time travel.
- I assume there are quite a few better strategies for checking and that my solution would not scale and so on and so forth. I wanted to always check the same group of hours to reduce the chance of user error (which I suspect to have played a major role in my previous attempts to identify my random seed having failed entirely.)
- I ended up using 2 days of normal playtime data, the dates of two meteor showers, and 7 days of time-travel data using this method. (I had older data as well from screenshots and the like, but previous attempts to use that data did not work.) This was enough for MeteoNook to identify what I believe to be my random weather seed. (I time-traveled to check double rainbows and heavy rain, and so far it _seems_ to be correct.) I have no idea if the search will be as quick for other folks, and it remains possible I messed up the data entry somewhere along the line.
