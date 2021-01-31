### Debugging
- What was the bug?
  - The variables `num1` and `num2` are strings so using `+` on them actually concatenates the both together resulting in the wrong behavior.

- How would you fix it? Include a screenshot of your fix.
  - I would typecast the strings to numbers before adding them with `+`.

### Network
- What is the name of the new json file?
  - `citylots.json`
- Which file initiated the download of the new file?
  - `part2.js`
- What is its file size?
  - `11.7MB`
- How long did it take to download?
  - `2.02s`
- What was your User-Agent for the browser that made the request?
  - `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.104 Safari/537.36`
- In the response, what type of server did it come from?
  - `Apache`
- When was the file last modified?
  - `Tue, 26 Jan 2021 22:14:13 GMT`
- What was the Content-Type of the file?
  - `application/json`
- Which method inside the initiating file made the request?
  - `fetchData()`