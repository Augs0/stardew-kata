# Do we need to water the crops? 🌽🌶️🍓🥔🥦🍇

This kata is inspired by the hugely popular game _Stardew Valley_, but does not require any knowledge of the game to complete. 💫

## Background 🗒️
You are a farmer in a small town. Every day, the crops must be watered so that they do not die. It does rain sometimes and those days we don't need to water the crops. The weather forecast isn't always right, but helps us to plan for the days we don't need to water the plants. 
- All seasons last 28 days. 
- There will always be a forecast for every day
- Each crop takes 1 sprinkle of water
- Your watering can contains enough water to water 40 crops.

## Tasks 🚜
### Level 1
Create a function that takes a weather forecast as an argument and returns the number of days we do not need to water the crops.

### Level 2
The second iteration of the function will require both a weather forecast and the number of crops on your farm as arguments. It should return the number of days we do not need to water the crops as well as how many 'sprinkles' of water are required for the season. This should be in the form of a string like `There are x days that you can skip watering your crops. You will need x sprinkles of water.`

### Level 3
For extra brownie points, can you return the amount of water in watering cans instead of sprinkles needed? This should be done by accepting a third optional argument in the second function you created that is `true` if the user wants cans of water as the measurement and `false` if they would like to see it in sprinkles.

You can create two separate functions if you like; one for level 1 and one for level 2 + 3 as they are slightly different in behaviour and arguments they take. Please also use TDD.

## Resources 🌾
See the `weather.js` file for two examples of a weather forecast for testing purposes. You are welcome to change the data if you want to test different cases. One includes rainy days, the other does not.
