# Drag Scroll

[Vanlina JavaScript 30](https://javascript30.com/)의 21번 토픽 과제 


## Discription
HTML5에서 제공하는 geolocation 프로퍼티에 대해 알아보고자 했고, Xcode의 Simulator를 이용하여 실행을 확인했다.

![image](https://github.com/ddinggu/compass/blob/master/screenshot.png?raw=true)



#### WatchPosition

watchPosition은 사용자의 GPS를 이용하여 사용자의 이동을 감지하여 성공(첫번째 매개변수)/실패(두번째 매개변수)시 해당하는 콜백함수가 실행되는 메소드이다. 

성공시 사용자의 위치에 따른 여러가지 정보들을 콜백함수에 position 객체로 넘겨줄 수 있고, 이 position 객체의 croodinates 객체 안에는 **위/경도 및 고도, 방향, 속도, 정확도** 값을 갖고 있다.

이러한 정보들을 이용하여 사용자 위치이동에 따른 여러 서비스들을 제공 할 수 있다. 

#### Style

watchPosition에 의해 사용자의 위치가 변할시, ```transform : rotate${heading}deg``` 를 이용해 이미지를 회전시켜 사용자의 방향을 알려줄 수 있도록 만들었다. 


#### Refernce 

https://developer.mozilla.org/ko/docs/Web/API/Geolocation/getCurrentPosition