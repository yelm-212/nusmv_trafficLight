# nusmv_trafficLight

![[TrafficLight.jpg]]

- state : Initial, On, Ready, Running, Off의 5가지 상태를 가질 수 있다고 가정한다
- On / Off를 결정하는 controller가 별도로 존재한다고 가정하고, Ready 상태에 진입했을 때 controller가 ON 이어야 ready 상태로 진입한다.
- controller가 OFF 이면, 이전 상태에서 Ready/ Running 의 어느 상태에 위치했더라도 ready 상태 로 진입한다.
- 추가 설정: time 의 값 법의는 0~ 60s이며,
(작동 시간 1시간) (오차 보정 위해 max값 80으로 설정)
그 이상 작동하면 OFF되도록 설계되었다고 가정하였다.
- Running State에서는 (light) color로 r, g , b를 가질 수 있다.
