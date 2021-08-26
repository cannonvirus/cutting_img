# 프로젝트명
> pig image cutter

<!-- [![NPM Version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Downloads Stats][npm-downloads]][npm-url] -->

rotated box 돼지 이미지를 RNN + Unet 계열의 모델을 돌리기 위해 데이터 전처리하는 코드

<!-- ![](../header.png) -->

## 설치 방법

Window :

```sh
pip install PyYAML
pip install pandas
pip install pandasql
```


## 사용 예제

우선 프레임별 돼지 정보(det_file_)이 있어야함
* /util/load_json.py : det_file_ 추출
<!-- * repo : [pig-tracking][pig-tracking] -->

### cutting_config.yaml
```sh
sample_img:
    img_folder_path: {이미지 폴더}
    det_file_path: {이미지 폴더에 매칭되는 detection 정보}
    img_format: ".jpg"
    det_format: ".txt"
    width_roi_padding: 0.08
    height_roi_padding: 0.0
    show_option: True # only window option [cv2.show]

cutting_img:
    output_path: {cutting된 이미지를 뽑을 폴더}
    width: 128
    height: 128
```


## 개발 환경 설정

Window 환경에서 구동완료


## 업데이트 내역

* master
    * readme.md 정리 완료


## 정보

주소현 – cannonvirus@intflow.ai


<!-- Markdown link & img dfn's -->
<!-- [pig-tracking]: https://github.com/cannonvirus/pig_tracking/tree/landmks_3 -->