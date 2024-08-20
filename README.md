# AIc

## 1. 프로젝트 개요
<아이크>는 영상 속 유해 정보와 개인정보를 모자이크하는 영상 자동 모자이크 서비스입니다.

### 주요 기능:
- 영상을 업로드하고 라벨을 고르면 선택된 라벨이 모자이크 된 영상을 얻을 수 있습니다.
- 실시간으로 유해 정보와 개인정보를 가릴 수 있는 실시간 모자이크를 제공합니다.
- 사용자 편의를 위해 챗봇과 문의 게시판을 제공합니다.

## 2. 파일 구조
이 프로젝트의 주요 디렉토리 및 파일 구조는 다음과 같습니다:

```
backend/
├── app.js
├── Dockerfile
└── package.json

config/
└── secrets.json

fastapi-f/
├── knn_examples/
├── logs/
│   ├── dlib_face_recognition_resnet_model_v1.dat
│   ├── Dockerfile
│   ├── main.py
│   ├── shape_predictor_68_face_landmarks.dat
│   ├── test_blur_app.py
│   └── trained_knn_model.clf
└── requirements.txt

fastapi-mp/
├── app/
│   ├── configdb.py
│   ├── database.py
│   ├── main.py
│   ├── models.py
│   └── video_processor.py
├── app2/
│   ├── main2.py
│   ├── downloads/
│   ├── logs/
│   └── processed_videos/
└── yolomodel/
    ├── addf2.pt
    ├── card2.pt
    ├── Dockerfile
    ├── Dockerfile.mongo
    ├── mongod.conf
    └── requirements.txt

fastapi-user/
├── app/
│   ├── main.py
│   ├── Dockerfile
│   ├── init.sh
│   ├── my.cnf
│   └── requirements.txt
└── frontend/
    ├── public/
    │   ├── images/
    │   ├── favicon.ico
    │   ├── index.html
    │   └── manifest.json
    └── src/
        ├── components/
        ├── routes/
        ├── App.css
        ├── App.js
        ├── App.test.js
        ├── index.css
        ├── index.js
        ├── PretendardVariable.ttf
        ├── reportWebVitals.js
        ├── TossFaceFontMac.ttf
        ├── .gitignore
        ├── config-overrides.js
        ├── Dockerfile
        ├── package-lock.json
        ├── package.json
        └── README.md
├── .env
├── .gitignore
├── docker-compose.yml
└── Makefile
```
