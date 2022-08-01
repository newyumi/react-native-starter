
# 앱 구동방법
## 공통
```
# 프로젝트 최상위 package.json 이 있는 위치에서 실행
yarn install
또는
npm install
```
## 빌드

```
# gradle 설정
rm -rf ~/.gradle
./gradlew clean

# apk 파일 추출
yarn build:apk && yarn open:apk

# 안드로이드 aab 파일
yarn build:aab && yarn open:aab
```

## ios
```
# yarn install 후 최초 실행 시
cd ios && pod install
# pod install 완료 후 다시 프로젝트 최상위 루트에서 아래 명령어 실행
npx react-native run-ios
```

## Android
```
# 프로젝트 최상위 루트에서
npx react-native run-android
```

위 빌드 방법은 React Native 환경 세팅이 우선 되어 있어야 합니다.
관련 내용은 아래 링크를 참조해주세요.

[React Native Environment Setup](https://reactnative.dev/docs/environment-setup)
