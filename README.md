# Inside The Dark
숭실대학교 졸업작품 3D 1인칭 멀티플레이 호러 게임


# 개요
프로젝트 이름: Inside The Dark

개발 기간: 2020.08.01 ~ 2021.05.23 

개발 인원: Tri 팀 윤민근, 이홍주, 박주연 (3명)

역할 분담: 윤민근, 이홍주, 박주연 모두 기획, 모델링, 3D 애니메이션, 개발, 최적화 진행


# 사용된 기술
- 사용 언어: C#
- 네트워크: Photon
- Unity
- Maya
- Fusion 360
- GitLab


# 게임 설명
대저택에서 발생하는 집주인과 좀도둑의 죽음의 술래잡기


# 게임 목적
집주인: 집에 몰래 칩입한 좀도둑을 칼로 3번 찔러 죽인다.

좀도둑: 집주인을 피해 화면 UI에 실루엣으로 제공된 3가지 물건을 훔치고 탈출한다.


# 게임 설계
공통 기능:
- 각자의 닉네임 설정 후 임의의 방 생성 및 입장
- 걷기, 뛰기, 점프, 웅크리기 가능
- 어두운 집에서 On/Off 가능한 손전등 제공
- 각자가 연 문과 손전등 빛이 공유되어 서로가 볼 수 있음
- 특정 구역 방문 시 효과음 발생
- 미니맵 제공 (단, 역할에 따라 제공되는 정보의 차이가 있음)

집주인 기능:
- 칼을 휘둘러 좀도둑을 공격할 수 있음 (공격 성공 시 쿨타임 발생)
- 달리기 바(Sprint Bar)가 있어서 소진 시 달리기에 제한 있음
- 아이템의 위치가 적힌 미니맵 제공 (단, 표시된 6개의 아이템 중 랜덤으로 좀도둑은 3개의 아이템만 훔침)
- 좀도둑이 아이템 훔칠 시 미니맵에 표시됨

좀도둑 기능:
- 하트 3개까지 있음
- UI에 훔쳐야 하는 물건의 실루엣이 출력
- 스킬 보유 (먹물 뿌리기와 투명화)
- 방과 문 표시만 있는 미니맵 제공


# 느낀 점
- 세 명 다 유니티를 이전에 사용한 적이 없어서 처음엔 막막했지만, 구글, 유튜브 등을 참고하여 해당 게임을 만들 수 있었습니다. 
- 기획서의 중요성을 깨달았습니다. 약 3~4개월 동안 기획을 탄탄히 다졌기 때문에 가끔 개발에서 헷갈리는 부분이 발생했을 때 기획서를 참고하며 다시 개발에 집중할 수 있었습니다.
- 인터넷에 Photon에 대한 자료가 부족하여 네트워크와 관련된 버그를 수정할 때 오랜 시간이 소요되었으나 이를 통해 멀티 게임의 원리를 더 잘 이해할 수 있었습니다.
- 실제로 문이 동기화되지 않아 플레이어 서로의 여닫는 문을 확인할 수 없는 치명적 버그가 존재했습니다. 하지만 PunRPC 프로시저를 사용하여 이를 해결했습니다.
- 전시 약 3주 전에 개발을 마치고 지인들을 통해 베타 테스트를 진행했습니다. 이 과정을 통해 제3자의 피드백을 받을 수 있었고 집주인과 좀도둑의 밸런스 등 부족함을 메꿨습니다.
- 최적화를 진행함으로써 게임의 용량과 로딩 시간을 효과적으로 줄일 수 있었습니다.
- 과연 남들에게 보여주기 떳떳한 작품을 만들 수 있을까 하는 우려로 시작했으나 3일 동안 400여명이 게임을 즐겨줘서 뿌듯했습니다.


# 인게임 화면
![Tri_titlePage](https://github.com/mingeun26/Grad_Project/assets/76557726/f112f5b9-cdb9-4f2c-a175-4c1ac2b06428)
![3게임설명](https://github.com/mingeun26/Grad_Project/assets/76557726/67754897-a94a-4b94-8f4d-5d4669d9a328)
![캐릭터 소개](https://github.com/mingeun26/Grad_Project/assets/76557726/b4e94327-dc47-47f8-a325-e7ad3d485178)
![키 설명](https://github.com/mingeun26/Grad_Project/assets/76557726/0a43e5c7-ebdb-4c80-9896-b540c56cc4bd)


#### [게임 로비]

![2로비사진](https://github.com/mingeun26/Grad_Project/assets/76557726/96f9bdc0-17fa-44da-b95f-0adb64a574c0)


#### [좀도둑 화면]

![좀도둑화면](https://github.com/mingeun26/Grad_Project/assets/76557726/e4671b93-575c-4ab8-8366-61f1b1d5583c)


#### [집주인 화면]

![집주인화면](https://github.com/mingeun26/Grad_Project/assets/76557726/90cecd7f-116a-4ceb-83c8-f0752dc1bb35)


#### [집주인 미니맵]

![집주인미니맵](https://github.com/mingeun26/Grad_Project/assets/76557726/4fdcfbe0-69be-4222-a379-26a119e9f71b)


#### [실제 플레이 사진]

![실제플레이_가림](https://github.com/mingeun26/Grad_Project/assets/76557726/30c57332-45d2-4b4c-963c-b26bca9ee0ad)


#### [대저택 인테리어]
![인게임2](https://github.com/mingeun26/Grad_Project/assets/76557726/4e9515d2-7f9d-4568-8ad8-41f2440e06ef)

![인게임사진](https://github.com/mingeun26/Grad_Project/assets/76557726/12ded0f5-5215-4dd7-9a57-1eb23abdaedd)

![좀도둑_화면](https://github.com/mingeun26/Grad_Project/assets/76557726/8e443092-3c9f-4383-998c-63f9c46c7a5f)

![인게임3](https://github.com/mingeun26/Grad_Project/assets/76557726/6b04b1e8-5d69-41e2-a4b9-2976471bc605)




