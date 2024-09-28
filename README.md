# Run Your City Impact Calculator

## Overview

The Run Your City Impact Calculator is a simple, web-based tool designed to estimate the potential impact of running programs on children in a community. This calculator is part of the Run Your City initiative, a non-profit organization that aims to build an inclusive community around the sport of running and foster children's growth into healthy, confident, and inspired individuals.

## Features

- User-friendly interface based on Material Design 3 principles
- Calculates estimated impact based on number of participants, program duration, and session frequency
- Provides results for total miles run, calories burned, potential confidence increase, and community engagement hours

## How to Use

1. Open the `index.html` file in a web browser.
2. Enter the following information:
   - Number of children participating
   - Program duration (in weeks)
   - Number of sessions per week
3. Click the "Calculate Impact" button to see the results.

## Calculations Explained

The calculator uses the following methods to estimate the program's impact:

1. **Total Miles Run**: 
   ```
   totalMilesRun = totalSessions * numChildren * 1.5
   ```
   Where `totalSessions = programDuration * sessionsPerWeek`
   We assume an average of 1.5 miles run per session per child.

2. **Calories Burned**:
   ```
   caloriesBurned = totalMilesRun * 100
   ```
   We estimate 100 calories burned per mile run.

3. **Confidence Increase**:
   ```
   confidenceIncrease = Math.min(programDuration * 2, 100)
   ```
   We estimate a 2% increase in confidence per week, with a maximum of 100%.

4. **Community Engagement Hours**:
   ```
   communityEngagementHours = totalSessions * numChildren
   ```
   This represents the total hours all children spend in the program.

## Implementation Details

- The calculator is implemented using HTML, CSS, and JavaScript.
- It uses Material Design 3 color principles for a modern, accessible interface.
- The calculations are performed client-side for immediate results.

## Contributing

We welcome contributions to improve the Run Your City Impact Calculator! Please feel free to submit issues or pull requests with your suggestions or improvements.

## License

This project is open source and available under the [MIT License](LICENSE).

---

Created with ❤️ by Run Your City
