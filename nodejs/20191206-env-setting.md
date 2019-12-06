1. download nodejs
https://nodejs.org/en/
Recommended for most users

2. version check
$ node -v
v12.13.1
$ npm -v
6.12.1

3. run to app
mkdir myapp
cd myapp
npm init
npm install express
vim index.js
```
const express = require('express')
const app = express();

app.get('/', (req, res) => {
  res.send('Hello World!')
});

app.listen(8000, () => {
  console.log('Example app listening on port 8000!')
});
```
$ node index.js

4. npm install eslint -D(좀 더 공부하고 사용)
ESLint는 사용자가 직접 정의한대로 코드를 점검하고, 에러가 있으면 표시해줍니다. 또 문법 에러뿐만 아니라 코딩 스타일도 정할 수 있어서 팀원끼리 협업을 할 때 좋습니다. 팀원끼리 협업을 하는 것과 코딩 스타일이 무슨 상관이 있을까요? 사람은 저마다의 코딩 스타일이 있기 때문에 여러 사람이 같이 코딩을 하면 차이가 발생합니다. 이럴 때 팀에서 하나의 코딩 스타일을 적용하고 ESLint에 설정해두면 마치 한 사람이 코딩을 한 것 같은 결과를 얻을 수 있습니다.

5. npm install express-generator -g
express helloworld
cd helloworld
npm install