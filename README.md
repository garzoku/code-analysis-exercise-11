# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input | Output        |
| ----- | ------------- |
|   1   | humanYears: 1,|
|       | catYears: 15, |
|       | dogYears: 15, | 
|   2   | humanYears: 2,|
|       | catYears: 24, |
|       | dogYears: 24, | 
|   3   | humanYears: 3,|
|       | catYears: 28, | 
|       | dogYears: 29, | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>1). The test input __actualAge__ is accepted by the function as an argument.<br>
2). If __actualAge__ is equal to 1, then the following code block is executed. __humanYears__ is assigned the value of __actualAge__, while __catYears__ and __dogYears__ are assigned a value of 15. This __object__ of values is then returned and the function is complete. If __actualAge__ is not equal to 1, the following code block will not be executed.<br>
3). If __actualAge__ is equal to 2, then the following code block is executed. __humanYears__ is assigned the value of __actualAge__, while __catYears__ and __dogYears__ are assigned a value of 24. This __object__ of values is then returned and the function is complete. If __actualAge__ is not equal to 2, the following code block will not be executed.<br>
4). If __actualAge__ is not equal to 1 or 2, it will skip the first two blocks and go straight to the third. __humanYears__ is assigned the value of __actualAge__. __catYears__ and __dogYears__ will be assigned the resulting values of (actualAge - 2) * 4 + 24 and (actualAge - 2) * 5 + 24, respectively.<br>
Summary: This function calculates how old a cat or dog is in their own "years" compared to a human of the __actualAge__ value.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
