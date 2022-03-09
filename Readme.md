# Readme
***
## 페이지 소개
Lorem과 간단한 CSS구현을 통해 제작한 웹 사이트

### **html**
특징 | 설명 | CSS
--|:--:|--:
Lorem | 내용 의미 없음|X
span|3개의 테두리 구성을 위해 사용함|O
a 태그|존재함|O
***
## CSS 
### **테두리제작 팁**  
1. `border-radius`를 4개가 아닌 8개를 주는 방법을 사용한다. 
    ```CSS
    border-radius: 40% 60% 65% 35% / 40% 45% 45% 60%;   
    ```
2. 애니메이션을 이용해 방향과 시간을 설정한다.
    ```CSS
    @keyframes ani {
      0% {
      transform: rotate(0);
      }

      100% {
      transform: rotate(360deg);
      }
    }
    ```
3. `hover`시 투명도를 이용해 구별
    ```CSS
      .container .square:hover span:nth-child(1) {
        opacity: 0.5;
      }

      .container .square:hover span:nth-child(2) {
        opacity: 0.8;
      }

      .container .square::hover span:nth-child(3) {
        opacity: 0.2;
      }
    ```