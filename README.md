# DFC615

1. 실험 환경 : Google colab 활용

2.학습 데이터 
  1. 한국어 감정 분석 
    • 영화 리뷰를 바탕으로 긍정/부정을 예측 
    • NSMC 다운로드 :  https://github.com/e9t/nsmc
      [ 학습 모델 - 나이브 베이즈, Tf-idf, 형태소 분석기, (1,2)-gram ]
        > 감성 분석이란 문서에 대해 좋다(positive) 혹은 나쁘다(negative)는 평가를 내리는 것
       샘플 데이터로는 github에 올려져 있는 네이버 영화 감상평에 대한 감성 분석 예제 이용
        > https://github.com/e9t/nsmc
      
      
  2. 영어 감정 분석 
    • 드라마 대본으로부터 감정을 분류 
    • Friends 데이터 다운로드  http://doraemon.iis.sinica.edu.tw/emotionlines/download.html
    [ 학습모델 ]
     양방향 LSTM을 가진 신경망을 감정 감지 데이터에 대해 훈련시키고 relu와 softmax를 활용하고 8가지의 감정으로 분류함
     dic = {'anger':0, 'disgust':1, 'fear':2, 'joy':3, 'neutral':4, 'non-neutral':5, 'sadness':6, 'surprise':7}
     


