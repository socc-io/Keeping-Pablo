# Keeping-Pablo
강화학습을 이용한 게임 인공지능

DQN을 이용한 간단한 게임을 플레이 하는 인공지능


기존에 있는 github 프로젝트 DeepFlappyBird의 소스코드를 이용하여 자체제작한 게임에 적용해 본 프로젝트

https://github.com/yenchenlin/DeepLearningFlappyBird

dependencies - tensorflow, opencv, pygame

```
pip install -r requirements.txt
python main.py
```

game.py 에서 frameStep마다 정의해주는 reward를 어떻게 정해주냐에 따라서 agent의 행동이 달라짐.
현재 정책으로는 세모에 부딪치면 -1점

도착지에 도착하면 1000점

도착지에 얼마나 가까우냐에 따라서 2단계로 나눈뒤 1단계에 해당하면 0.1점, 2단계에 해당하면 0.5점을 부여함.
