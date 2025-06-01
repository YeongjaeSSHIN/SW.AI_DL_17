# DL_Project_17

DATASET: https://archive.org/details/idrid
Segmentation Model 생성을 위해 위 데이터 중 A.Segmentation을 사용.
A. segmentation
- 1. Original Images (Images)
     - train
     - test
  2. All Segmentation groundtruths (Masks.tif)
     - train
       - Microaneurysms
       - Haemorrhages
       - Hard Exudates
       - Soft Exudates
       - Optic Disc (정상조직)
     - test
위 데이터 중, Optic Disc 제외하고 사용, .tif 형식으로 [0 (비병변), 76 (병변)] 형태임 -> 이걸 .png로 변환하기 위해 [0, 255]로 변환, 그리고 .png로 변환

## Segmentation model
https://github.com/YaqiWangCV/LKD.git (병변 종류별로 X, 병변인 부분과 정상 조직을 1과 0으로 segmentation)

https://dl.acm.org/doi/abs/10.1007/s10489-024-05274-8

https://drive.google.com/drive/folders/11FbKatIlVzWhyOtFAhn8CVhP_qWFSkCh?usp=drive_link

## Segmentation model 사용해서 feature 추출

## Grading model
https://github.com/chehx/DGDR/tree/main
