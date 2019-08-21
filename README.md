# Learning-Javascript

Learning Javascript 책을 보면서 공부한 내용과 혼자 찾아가며 공부한 내용을 정리

> 저자 : 이선 브라운
>
> 번역 : 한선용
>
> 출판사 : 한빛미디어

## 주석 

  ```javascript
  console.log("echo") // 콘솔에 echo를 출력
  
  /*
  자바스크립트 주석
  자바의 주석과 동일
  */
  ```
 
## HTML에서 CSS와 JavaScript, JQuery 불러오는 방법 
 
  ```html 
<!doctype html>
<html>
    <head>
        <!-- CSS 파일을 문서로 불러오는 링크 -->
        <link rel="stylesheet" href="main.css">
    </head>
    <body>
        <!-- JQuery 파일을 문서로 불러오는 링크 -->
        <script src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
        <!-- JavaScript 파일을 문서로 불러오는 링크 -->
        <script src="main.js"></script>
    </body>
</html>
  ```
  
 ## console 
 
  cosole은 프로그램을 진단할 때 사용하는 텍스트 전용 도구입니다. console은 개발자 도구(F12)에 내용을 출력하고 싶을 경우 사용할 수 있습니다.
  console에 지정할 수 있는 속성이 여러가지 있는데 대표적으로 `log`와 `dir`가 있습니다.

  console을 사용하고나서 개발자 도구(F12)를 눌러서 console에 들어가면 console로 출력한 내용을 볼 수 있습니다.
  
  - console.log
  
   ```javascript
   console.log(document.querySelector('.inner'));
   ```
   
   - 개발자 화면에 출력되는 모양 
   
   ```html
  <table class="table">
      <thead>
            <tr>
                <th>수정 날짜</th>
                <th>복구</th>
            </tr>
        </thead>
  </table>
  ```
  
  - console.dir 
  
  ```javascript
  console.dir(document.querySelector('.inner'));
  ```
  
   - 개발자 화면에 출력되는 모양(객체형식)
   
   ```
  accessKey: ""
  align: ""
  assignedSlot: null
  attributeStyleMap: StylePropertyMap {size: 0}
  attributes: NamedNodeMap {0: class, class: class, length: 1}
  ```

## babel 

   자바스크립트의 최신문법인 ES6와 ES7을 사용하여 브라우저에 인식시키기 위해서는 `babel`이라는 자바스크립트 컴파일러가 필요합니다. 입력은 자바스크립트 코드이며, 출력도 자바스크립트 코드 입니다.
   
   즉, `최신 버전의 자바스크립트 문법(ES6, ES7)`은 브라우저가 이해하지 못하기 때문에 babel이 브라우저가 이해할 수 있는 문법으로 변환해줍니다. ES6, ES7 등의 최신 문법을 사용해서 코딩을 할 수 있기 때문에 생산성이 향상된다.
   
   > ECMAScript5 : 브라우저가 이해할 수 있는 자바스크립트 문법
   
   Babel은 아시다시피 ES6/ES7 코드를 ECMAScript5 코드로 transpiling 하기 위한 도구입니다. Babel은 다양한 작은 모듈들로 구성되어 있습니다. Babel 다양한 모듈을 담는 일종의 상자 역할을 하며 코드를 컴파일 하기 위해 작은 모듈들(ex. presets)을 사용합니다.
  

