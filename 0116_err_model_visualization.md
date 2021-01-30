## err , problem data EDA

### 1. 모델 변경 횟수 분포 확인    
          train                      test
<p>
<img src="./img/0116/train_model_count.png" width="200" height="100" >
<img src="./img/0116/test_model_count.png" width="200" height="80" >
</p>


- 모델 변경은 순차적으로 일어난다. a모델 사용시기 종료 -> b 모델 사용
- 1번 모델을 바꾼 사람의 경우 (641/700) ->91%의 확률로 불만 제기
- 2번 모델을 바꾼 사람의 경우 (2/3)-> 불만 제기 -> 이중 불만제기 2명(13991,20921)은 a모델 -> b 모델 -> a모델
  
- 파생변수로서 매우 적절해보임 (모델변경 횟수)
  

******


### 모델 변화의 경향
# 
- train
<p>
<img src='./img/0117/img_train_model_change.png' width='500',height='100' , aline='center'>
</p>
- test
<p>
<img src='./img/0117/img_test_model_change.png' width='500',height='100'>
</p>


*****
### 모델변화 700명의 에러 발생시점 (발생시점에 따른 sorting)
# 

<p>
<img src='./img/0117/pb_occur.png' width='1200',height='400'>
</p>

모델이 바뀌는 시점에서 problem occur이 많이 발생하는 것을 확인 할 수 있다.    
파생변수로 선택하기 적합해보임 

# 
### plot 자료 및 다음 스텝
- Model 과 Errtype에 따른 problem non-problem 유저들의 err 발생 시점을 확인
- model의 경우 1,2,3,4번이 p - np 차이가 뚜렷해보임
- errtype의 경우 1,3,4,5,6,7,10,11,12,17,22,23,24,27,28,32,34 p -np 차이보임
- 이들을 통한 파생변수생성 해야할것
- 전체 주차 대비 각 주차의 errtype 빈도 등을 만들 예정 -> 우선 p - np 의 각 타입별 통계적 차이 검정
- 


#   
### model 별 problem 발생시점
                                            model 0 
<p>
<img src='./img/model_type/model_0.png'>
</p>

                                            model 1
<p>
<img src='./img/model_type/model_1.png'>
</p>

                                            model 2 
<p>
<img src='./img/model_type/model_2.png'>
</p>

                                            model 3 
<p>
<img src='./img/model_type/model_3.png'>
</p>

                                            model 4 
<p>
<img src='./img/model_type/model_4.png'>
</p>

                                            model 5 
<p>
<img src='./img/model_type/model_5.png'>
</p>

                                            model 6 
<p>
<img src='./img/model_type/model_6.png'>
</p>

                                            model 7 
<p>
<img src='./img/model_type/model_7.png'>
</p>

                                            model 8 
<p>
<img src='./img/model_type/model_8.png'>
</p>

*****
### errtype별 problem 발생시점
                                            err 1 
<p>
<img src='./img/err_type/1.png'>
</p>        

                                            err 2
<p>
<img src='./img/err_type/2.png'>
</p>

                                            err 3
<p>
<img src='./img/err_type/3.png'>
</p>

                                            err 4
<p>
<img src='./img/err_type/4.png'>
</p>

                                            err 5
<p>
<img src='./img/err_type/5.png'>
</p>

                                            err 6
<p>
<img src='./img/err_type/6.png'>
</p>

                                            err 7
<p>
<img src='./img/err_type/7.png'>
</p>

                                            err 8
<p>
<img src='./img/err_type/8.png'>
</p>

                                            err 9
<p>
<img src='./img/err_type/9.png'>
</p>

                                            err 10
<p>
<img src='./img/err_type/10.png'>
</p>

                                            err 11
<p>
<img src='./img/err_type/11.png'>
</p>

                                            err 12
<p>
<img src='./img/err_type/12.png'>
</p>

                                            err 13
<p>
<img src='./img/err_type/13.png'>
</p>

                                            err 14
<p>
<img src='./img/err_type/14.png'>
</p>

                                            err 15
<p>
<img src='./img/err_type/15.png'>
</p>

                                            err 16
<p>
<img src='./img/err_type/16.png'>
</p>

                                            err 17
<p>
<img src='./img/err_type/17.png'>
</p>

                                            err 18
<p>
<img src='./img/err_type/18.png'>
</p>

                                            err 19
<p>
<img src='./img/err_type/19.png'>
</p>

                                            err 20
<p>
<img src='./img/err_type/20.png'>
</p>

                                            err 21
<p>
<img src='./img/err_type/21.png'>
</p>

                                            err 22
<p>
<img src='./img/err_type/22.png'>
</p>

                                            err 23
<p>
<img src='./img/err_type/23.png'>
</p>

                                            err 24
<p>
<img src='./img/err_type/24.png'>
</p>

                                            err 25
<p>
<img src='./img/err_type/25.png'>
</p>

                                            err 26
<p>
<img src='./img/err_type/26.png'>
</p>

                                            err 27
<p>
<img src='./img/err_type/27.png'>
</p>

                                            err 28
<p>
<img src='./img/err_type/28.png'>
</p>

                                    err 29 은 train_test 모두 없음

                                            err 30
<p>
<img src='./img/err_type/30.png'>
</p>

                                            err 31
<p>
<img src='./img/err_type/31.png'>
</p>

                                            err 32
<p>
<img src='./img/err_type/32.png'>
</p>

                                            err 33
<p>
<img src='./img/err_type/33.png'>
</p>

                                            err 34
<p>
<img src='./img/err_type/34.png'>
</p>

                                            err 35
<p>
<img src='./img/err_type/35.png'>
</p>

                                            err 36
<p>
<img src='./img/err_type/36.png'>
</p>

                                            err 37
<p>
<img src='./img/err_type/37.png'>
</p>

                                            err 38
<p>
<img src='./img/err_type/38.png'>
</p>

                                            err 39
<p>
<img src='./img/err_type/39.png'>
</p>

                                            err 40
<p>
<img src='./img/err_type/40.png'>
</p>

                                            err 41
<p>
<img src='./img/err_type/41.png'>
</p>

                                            err 42
<p>
<img src='./img/err_type/42.png'>
</p>