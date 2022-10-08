# Electron 예제

### electron.js 파일을 /public 에 넣은 이유?

public 폴더에 만드는 이유는 electron-builder가 패키징 할 때 create-react-app이 build 한 build 폴더를 패키징 하는데

이때 electron 앱의 엔트리 포인트가 없는 상태가 됩니다.

그래서 public 폴더에 electron 앱의 엔트리 포인트인 electron.js를 만들면 create-react-app의 webpack이 자동으로 public 폴더를 build 폴더에 복사하기 때문에 electron-builder 가 패키징 할 수 있게 됩니다.

그리고 electron.js라고 이름 지은 이유는 electron-builder 가 디폴트로 일렉트론 앱의 엔트리 포인트로 build/electron.js 파일을 찾기 때문입니다.
