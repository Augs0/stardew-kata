# Do we need to water the crops? 🌽🌶️🍓🥔🥦🍇

This kata is inspired by the hugely popular game _Stardew Valley_, but does not require any knowledge of the game to complete. 💫

## Background 🗒️
You are a farmer in a small town. Every day, the crops must be watered so that they do not die. It does rain sometimes and those days we don't need to water the crops. The weather forecast helps us to plan for the days we don't need to water the plants. 
- All seasons last 28 days. 
- There will always be a forecast for every day.
- Each crop takes 1 sprinkle of water.
- Your watering can contains enough water to water 40 crops.

## Tasks 🚜
### Level 1
Create a function that takes a weather forecast as an argument and returns the number of days we do not need to water the crops. The function should take a full forecast of 28 days - that means no single days or missing days need to be considered.

```
function cropWateringCalendar([
    {day: 1, weather: "sunny"},
    {day: 2, weather: "sunny"},
    {day: 3, weather: "sunny"},
    {day: 4, weather: "clear"}...
])
```
The full 28 days will be input as above in an array of objects. We expect the output to be a number. For example, `0` if there are no rainy days or `4` if there are 4 rainy days in the forecast.

### Level 2
The second iteration of the function will require both a weather forecast and the number of crops on your farm as arguments. Please create a new function separate from the first.

For example:

```
function cropWateringCalendar([
    {day: 1, weather: "sunny"},
    {day: 2, weather: "sunny"},
    {day: 3, weather: "sunny"},
    {day: 4, weather: "clear"}...
], 10)
```
The above would be the full 28 day forecast and a number that represets the crops on the farm. In this case, there are 10 crops.

This function should return the number of days we do not need to water the crops as well as how many 'sprinkles' of water are required for the season. 

This should be in the form of a string like `There are x days that you can skip watering your crops. You will need x sprinkles of water.`

### Level 3
For extra brownie points, can you return the amount of water in watering cans instead of sprinkles needed? This should be done by accepting a third optional argument in the second function you created that is `true` if the user wants cans of water as the measurement and `false` if they would like to see it in sprinkles. _Remember_, your watering can holds enough water for 40 crops.

For example:

```
function cropWateringCalendar([
    {day: 1, weather: "sunny"},
    {day: 2, weather: "sunny"},
    {day: 3, weather: "sunny"},
    {day: 4, weather: "clear"}...
], 10, true)
```

Here, true has been passsed so our return value should measure the water by cans e.g. `There are x days that you can skip watering your crops. You will need x cans of water.`

Please also use TDD througout these tasks.

## Resources 🌾
See the `weather.js` file for two examples of a weather forecast for testing purposes. You are welcome to change the data if you want to test different cases. One includes rainy days, the other does not.
