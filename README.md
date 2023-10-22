# hotelreviewkor

# KOELECTRA를 활용한 호텔리뷰 평점 감성 분석

# 1. 개요
이 프로젝트의 목적은 KOELECTRA를 활용하여 호텔 리뷰의 감성을 분석하는 것입니다.<br> 
호텔 리뷰는 호텔 예약 고객에게 중요한 정보를 제공하는 주요 소스로 사용됩니다. 이러한 리뷰를 통해 호텔의 품질, 서비스 및 시설에 대한 정보를 얻어 만족할만 예약이 가능합니다.

## 1.1 문제 정의
호텔 리뷰는 호텔 예약에 있어 가장 보편적으로 활용되는 정보의 창구이다.
- 호텔 리뷰와 해당 호텔 성행의 상관관계를 나타내는 참고자료를 통해 호텔 리뷰의 가치를 언급
- [[1]](링크) 등의 표기를 문장 뒤에 활용하여 참고 문헌을 작성할 것
- 프로젝트로 해당 과업을 해결할 때 기대할 수 있는 장점, 활용 가능성 등을 언급
- 필요에 따라서는 적절한 그림을 그려 표현(ppt 등)

## 1.2 데이터 및 모델 개요
데이터는 네이버에서 제공하는 영화 리뷰를 활용[2]하여, 총 20만 건의 데이터에 대해서 사전 학습 언어 모델의 재학습(fine-tuning)을 수행한다.


|reviews|'star'|'label'|
| --- | --- | --- |
| 호텔리뷰 | 평점 | 긍정0,부정1 |
| 최고의 주말 데이트를 했습니다 | 5 | 0 |
| 야경이 너무너무 멋졌어요^^ | 5 | 0 |
| 친절하고 시설도 좋네요 | 5 | 0 |
| 체크인 시간 전에 도착 시 대기 할 공간이 미흡했던 것같고, 시설 이용할 수 있는게 한정적이여서 아쉬움이 컸음 | 4 | 0 |
| 나쁘잔않지만 가성비를따지자면 그닥.. | 3 | 1 |
| 서비스가 다 따로노는 느낌이네요..기대하고 간곳인데 기대이하네요 | 3 | 1 |
| 배드 밑에 뭘 깔아놓으셨는지 울퉁불퉁해서 허리아파서 잠을 못잤네요 | 1 | 0 |
| 개인 위생용품 자체가 없고, 냉방과 난방 둘 중 하나만 선택 가능합니다. | 2 | 0 | <br>

1. 엑셀내에서 쓸모없는 Unnamed, hotel(호텔이름), date(리뷰남긴날짜),real_date(실제 날짜)를 제거
2. 평점 "1~3"점은 부정(1), "4~5"점은 긍정(0)으로 변환




호텔 리뷰 문장은 전처리를 통해서 가공한다. 대표적인 전처리로는 결측치와 중복값을 제거하고, 띄어쓰기로 구분이 되지 않는 리뷰 역시 제거한다.

# 2. 데이터
## 2.1 데이터 소스

## 2.2 탐색적 데이터 분석

## 2.3 데이터 전처리
- 입력 데이터의 전처리 과정
- 학습에 활용할 데이터의 양
- 학습과 검증 데이터셋 분리
- 학습 데이터의 구성

# 3. 재학습 결과
## 3.1 개발 환경
- pycharm, python, torch, pandas, ...
-
## 3.2 KOELECTRA fine-tuning
## 3.3 학습 결과 그래프

# 4. 배운점
