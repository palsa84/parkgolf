설치 전 **저장공간** 확보하세요.

expo가 아닌 react-native cli와 npm 명령어로 Visual Studio Code에서 개발합니다.   
.ts, .tsx, kotlin, flutter가 아닌 .js, .jsx, react-native로 Android만 개발합니다.


## 안드로이드 스튜디오 설치
[https://velog.io/@completed1991/%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C-%EC%8A%A4%ED%8A%9C%EB%94%94%EC%98%A4-%EC%84%A4%EC%B9%98-%EB%B0%8F-%ED%99%98%EA%B2%BD%EB%B3%80%EC%88%98-%EC%85%8B%ED%8C%85](https://yun5o.tistory.com/entry/React-Native-%EB%A6%AC%EC%95%A1%ED%8A%B8-%EB%84%A4%EC%9D%B4%ED%8B%B0%EB%B8%8C-%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EC%84%A4%EC%A0%955-%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C-%EC%8A%A4%ED%8A%9C%EB%94%94%EC%98%A4-%EC%84%A4%EC%B9%98)

위 링크를 참고하여 다운 받고 환경변수까지 설정하세요.


## 설치 후 실행 
좌측하단 '설정 아이콘' -> 'About' 
아래 이미지와 똑같이 설정하세요.
![image](https://github.com/user-attachments/assets/86b77c4f-d3bf-4f39-a367-b963ec8a3068)




More Actions -> Virtual Device Manager
상단 + 버튼을 누르고 디바이스를 생성하세요.
Pixel 7, VanillaIceCream만 설정하면 됩니다.
![image](https://github.com/user-attachments/assets/79ed7002-dbfd-4e48-8fc1-867aff321c0a)
재생 버튼을 눌러 안드로이드 시뮬레이터가 정상적으로 작동하는지 테스트하세요.


More Aciton -> SDK manager에서 아래 이미지의 툴을 설치하세요.
![image](https://github.com/user-attachments/assets/27a98551-8c80-433d-95c4-6b492358355b)
![image](https://github.com/user-attachments/assets/13668a4a-e41f-4f2f-b226-a9b648b59f00)
![image](https://github.com/user-attachments/assets/2f57ac28-0d80-46e8-8953-97ed8eb344e6)
![image](https://github.com/user-attachments/assets/9ac9d4e1-604e-4a44-9d62-1942ab09aca0)




## Visual Studio Code 설치
v: 1.97.2
설치 후 프롬프트에서 아래 명령어 입력후 1.97.2가 뜨면 됩니다.
```sh
code --version
```


**업로드 된 코드를 .zip로 설치 및 압축해제 후 project1 폴더를 VScode에서 project1 폴더를 여세요.**

아래 이미지처럼 뜨는지 확인하세요.
![image](https://github.com/user-attachments/assets/2850b2b3-fd7d-40d6-a55b-d15fd58867a4)


**새 터미널(powershell) 생성**
아래 react-native cli 설치 명령어를 순차적으로 실행하세요.

```sh
npm install -g react-native-cli
```

```sh
npm install -g react-native
```

## java(jdk), react-native, npm, node, gradle을 아래 버전으로 설치하세요.
![image](https://github.com/user-attachments/assets/8ff2d801-c5eb-4481-ae0b-1408fed4c62a)

버전이 안 맞으면 다운그레이드하세요.


## 아래 명령어를 터미널에 입력하여 package.json 파일에 있는 모듈을 모두 설치하세요.
```sh
npm install @react-native-community/datetimepicker @react-native-seoul/kakao-login @react-navigation/native @react-navigation/native-stack @react-navigation/stack formik postcss react react-dom react-native react-native-gesture-handler react-native-reanimated react-native-safe-area-context react-native-screens react-native-vector-icons styled-components
```

```sh
npm install --save-dev @babel/core @babel/preset-env @babel/runtime @react-native-community/cli @react-native-community/cli-platform-android @react-native-community/cli-platform-ios @react-native/babel-preset @react-native/eslint-config @react-native/metro-config eslint jest prettier react-test-renderer
```

```sh
npx expo install react-native-screens react-native-gesture-handler
```

```sh
npm install
```



## 실행
project1 파일에서 실행하세요
```sh
cd project1
```

```sh
npm start
```

에러 뜨면 gpt로 해결하세요.

screens/Login.js, Signup.js, Welcome.js와 components/styles.js에만 주석 달아놨습니다. 확인하세요.
의존성 문제는 모듈마다 버전이 일치하지 않아서 뜨는 에러이므로 package.json의 버전을 확인하여 설치하여 주세요.
ex) npm install styled-components@버전번호



### 현재 에러
1. Signup 화면에서 캘린더(DateTimePIcker)



This is a new [**React Native**](https://reactnative.dev) project, bootstrapped using [`@react-native-community/cli`](https://github.com/react-native-community/cli).

# Getting Started

> **Note**: Make sure you have completed the [Set Up Your Environment](https://reactnative.dev/docs/set-up-your-environment) guide before proceeding.

## Step 1: Start Metro

First, you will need to run **Metro**, the JavaScript build tool for React Native.

To start the Metro dev server, run the following command from the root of your React Native project:

```sh
# Using npm
npm start

## Step 2: Build and run your app

With Metro running, open a new terminal window/pane from the root of your React Native project, and use one of the following commands to build and run your Android or iOS app:

### Android

```sh
# Using npm
npm run android


If everything is set up correctly, you should see your new app running in the Android Emulator, iOS Simulator, or your connected device.

This is one way to run your app — you can also build it directly from Android Studio or Xcode.

## Step 3: Modify your app

Now that you have successfully run the app, let's make changes!

Open `App.tsx` in your text editor of choice and make some changes. When you save, your app will automatically update and reflect these changes — this is powered by [Fast Refresh](https://reactnative.dev/docs/fast-refresh).

When you want to forcefully reload, for example to reset the state of your app, you can perform a full reload:

- **Android**: Press the <kbd>R</kbd> key twice or select **"Reload"** from the **Dev Menu**, accessed via <kbd>Ctrl</kbd> + <kbd>M</kbd> (Windows/Linux) or <kbd>Cmd ⌘</kbd> + <kbd>M</kbd> (macOS).
- **iOS**: Press <kbd>R</kbd> in iOS Simulator.

## Congratulations! :tada:

You've successfully run and modified your React Native App. :partying_face:

### Now what?

- If you want to add this new React Native code to an existing application, check out the [Integration guide](https://reactnative.dev/docs/integration-with-existing-apps).
- If you're curious to learn more about React Native, check out the [docs](https://reactnative.dev/docs/getting-started).

# Troubleshooting

If you're having issues getting the above steps to work, see the [Troubleshooting](https://reactnative.dev/docs/troubleshooting) page.

# Learn More

To learn more about React Native, take a look at the following resources:

- [React Native Website](https://reactnative.dev) - learn more about React Native.
- [Getting Started](https://reactnative.dev/docs/environment-setup) - an **overview** of React Native and how setup your environment.
- [Learn the Basics](https://reactnative.dev/docs/getting-started) - a **guided tour** of the React Native **basics**.
- [Blog](https://reactnative.dev/blog) - read the latest official React Native **Blog** posts.
- [`@facebook/react-native`](https://github.com/facebook/react-native) - the Open Source; GitHub **repository** for React Native.
