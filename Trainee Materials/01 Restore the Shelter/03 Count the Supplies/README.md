# 03 — Count the Supplies

**Chapter:** Restore the Shelter

**Work:** self-guided, individual, and AI-free. Use fictional exercise data only.

**Start here:** Complete Activity 02 first. Continue the same project.

## Mission briefing

The shelter has 18 water units. Six survivors each need two units per day. Command wants a reliable calculation before rationing begins.

## Learn: values, names, and calculations

```javascript
const batteryCount = 4;
const chargePerBattery = 3;
const availableCharges = batteryCount * chargePerBattery;
console.log("Available charges:", availableCharges);
```

Predict the output before running this smaller example. `const` binds a name that is not reassigned; JavaScript still permits mutation inside an object. Numbers and strings behave differently: compare `2 + 3` with `"2" + "3"` in the browser console and explain the results.

## Build it

1. Create a `js` folder inside `web`, then create `main.js` in it. In the head of `web/index.html`, add `<script src="js/main.js" defer></script>`. The relative path identifies the script; defer runs it after the HTML is parsed.
2. Define named values for water units, survivor count, and units needed per survivor per day.
3. Daily demand is survivor count multiplied by daily allowance. Complete days are `Math.floor(waterUnits / dailyDemand)`. Leftover is starting stock minus complete days multiplied by daily demand. Use names that match your own declarations; do not paste an undefined example variable.
4. Log clearly labeled results with console.log, save, open the page, and open browser developer tools → Console. Reload to rerun the script. No user input is required yet.
5. Change only the starting data to check another scenario; do not hard-code result strings.

## Independent task

Repeat the calculation for 25 food units, four survivors, and two units per survivor per day. Your independent food check should yield daily demand8, complete days3, leftover1. If it differs, trace the formula rather than changing the expected result. Keep water and food variable names clear. Add a short explanation of division, rounding, and remainder in `docs/activity-03.md`.

## Check and expected output

| Water units | Survivors | Units per day per survivor | Daily demand | Complete days | Leftover |
| ---: | ---: | ---: | ---: | ---: | ---: |
| 18 | 6 | 2 | 12 | 1 | 6 |
| 24 | 6 | 2 | 12 | 2 | 0 |
| 0 | 6 | 2 | 12 | 0 | 0 |

Use valid numeric inputs in this mission and compare them with the table above. Record zero survivors as an invalid input to handle in Activity 04; Infinity/NaN is not a useful answer.

## Troubleshooting

- No console output: save the script and HTML, check the exact js/main.js path, and reload. A Network404 means the file path is wrong.
- A ReferenceError means a variable name is misspelled or used before its declaration. A SyntaxError often points to a missing quote, parenthesis, or brace.
- A result looks like23 instead of5: inspect whether the inputs are strings.
- A fractional day is shown: apply Math.floor to days, then calculate leftover from those complete days.

## Git checkpoint

Use your existing Git workflow to inspect the changed files, stage only the intended source/notes, review the staged diff, commit with a useful message, and push to personal `main`.

Record the commit or PR link and your checks in `docs/activity-03.md` (create the docs folder if needed). Do not upload personal details or private answer keys. A local commit alone is not on GitHub.

Reference: [JavaScript numbers and operators](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/Math).

Return to the [chapter briefing](../README.md).
