https://github.com/dayoonkang/3_AnimalMatch/assets/150164152/15101331-d302-4865-8b1a-4a5a7976c820

# 🎮 AnimalMatch_2D_Mouseplay
유니티 2D 카드 맞추기 기억력 게임 "Animal Match"

## 💻 프로젝트 소개
제한 시간 50초 내에 모든 카드의 짝을 맞추는 마우스클릭 카드 맞추기 게임입니다.

게임을 시작하면, 5초동안 카드의 정답을 보여줍니다! ⏲️

원숭이, 쥐, 코끼리, 사자, 악어, 기린, 고양이, 거북이, 하마, 강아지 총 10종류의 동물 친구들이 두장씩 있어요. 🦛🐕🐈🦒🐢🐁🐒🦁🐘🐊

동물 친구들의 위치를 기억하고, 같은 카드 두장을 클릭해보세요! 🖱️💥

같은 그림이 맞다면🙆‍♂️, 성공! 틀리면🙅‍♂️ 카드는 다시 뒤집어져요. 


## 🏃‍♀️ 개발 기간
23.11.15 - 23.11.21

## ⚙️ 개발 환경 및 사용 언어
- Window x64
- Unity 2022.3.12f1
- Visual Studio 2022 C#

## 🌟 주요 기능
- 게임 시작 시, 5초간 정답 카드 공개
- 50초의 타임리밋, 줄어드는 Slider와 Text 
- 같은 카드라고 하면, 뒤집힌 채로 유지, 재 클릭 불가
- 다른 카드라고 하면, 다시 뒤집어짐, 재 클릭 가능
- 카드가 뒤집히는 모션을 scale/ticktime을 계산하여 조절
- GameBoard index와 card index를 설정하여 매 판마다 랜덤한 카드 위치 설정
- 50초 내에 모두 찾으면 성공, 남은 카드가 있으면 실패
- End Game Widget에서 성공/실패 여부 확인, Restart Button

## 💪 이 프로젝트를 통해 무엇을 배우셨나요?
- 필요한 에셋을 무료 저작권 사이트에서 다운로드하여 활용
- 이미지 Padding/Offset 값을 설정하여 이미지 Slice
- 카드가 뒤집어지는 효과: C#에서 변수를 생성하여 state 확인, Vector Scale을 변경하는 로직 작성
- 카드의 앞면과 뒷면 생성: C#에서 MouseClickDown 했을 때의 statement를 작성하여 Sprite Renderer를 통해 이미지가 변경되도록 처리
- 게임보드 설정: C#에서 게임보드의 row와 col의 위치를 연산하여 함수를 만들어 배치
- 랜덤으로 카드 배치: 랜덤 인덱스를 이용, 보드의 랜덤 인덱스와 카드 ID를 매치하여 저장하게끔 설정
- GameManager: 전체 게임의 흐름을 작성하는 GameManager.cs 파일을 생성, 5초간 모든 카드를 보여주는 기능, gameplay, endgame을 총괄
- 매치 확인: GameManager에서 카드를 클릭했을 때 뒤집힌 카드의 정보를 저장 (Debug.Log(")) 활용
- 매치 시 작동: 매치 성공 시/ 실패시 함수 및 bool 변수를 생성하여 클릭 이벤트를 설정
- 시간 제한: Slider를 생성, GameManager에서 Time.deltaTime 로직 작성, 몇초가 남았는지 Slider 옆 Text에 표시
- 게임 종료: 성공시와 실패 시의 Text 를 bool 변수를 사용하여 branch 나누어 표시, button 과 button click event 생성

## 💭 나중에 추가하고 싶은 기능
- 시작 시 StartGame/ Exit 창으로 진입, 시작하는 타이밍 설정 가능하게끔 구현
- Easy-Normal-Hard Mode 구현: 더 많은 카드, 더 짧은 플레이 시간, 더 짧은 카드 미리보기 시간 선택
- 플레이 사운드: 카드와 어울리는 깜찍한 플레이 사운드로 재미 up
- Hint 제공: hint button 클릭 시 한 쌍의 카드의 정답을 뒤집어서 보여주고 다시 뒤집어짐

## ✔️ 참고자료
Youtube - 나도코딩 "무조건 유용한 기억력 테스트 게임 - 유니티 게임개발 무료 강의 (실전 프로젝트2)"
