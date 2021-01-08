# Mac terminal **zsh** 설정하기

> 터미널을 사용하기에 앞서, 새로운 테마를 적용해보기



## **1. zsh 설치하기**

> 기본 `bash shell` -> `zsh`로 바꾸기

 - `Home-brew` 이용하여 설치

   (1) brew 버전 확인

   ```shell
   $ brew --version
   ```

   (2) brew update (필요 시)

   ```shell
   $ brew update
   ```

   (3) zsh install

   ```shell
   $ brew install zsh
   ```

   (4) zsh path 확인

   ```shell
   $ which zsh
   ```

   (5) 기본 `bash shell` 을 `zsh` 로 변경

   ```
   $ chsh -s $(which zsh)
   ```

   

## 2. Oh-my-zsh 설치

> `zsh` 환경 설정을 위한 프레임워크 `oh-my-zsh` 설치하기

  - [`oh-my-zsh` 설치 안내 페이지](https://ohmyz.sh/)

  - 설치 완료 후 화면

    ![zshell 설치 완료](/Users/spring/Desktop/스크린샷 2021-01-08 오후 9.06.39.png)



## 3. Theme 변경

- Default Theme :  `robbyrussell`

- Theme 변경을 위해 `.zshrc` 파일을 수정해야 함

  *.zshrc는 루트경로에 숨김파일로 존재*

- vscode로 파일 열기

  ```shell
  $ code .zshrc
  ```

![.zshrc](/Users/spring/Desktop/스크린샷 2021-01-08 오후 10.46.57.png)

- `ZSH_THEME` 를 원하는 Theme 로 변경
  - [`zsh_theme 종류`](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)

### 재미있는 기능 : `random theme`

- 특정 Theme로 설정하지 않고 Terminal을 실행할 때마다 Theme를 랜덤으로 사용해 볼 수 있는 기능

- 적용된 Theme 확인 방법

  - Terminal 상단에서 `[oh-my-zsh] Random theme 'Theme name' loaded`로 안내해줌

  - 상단의 random theme 메시지를 제거하고 싶다면

    -> [random theme 메시지 제거 방법](https://velog.io/@hwang-eunji/%ED%84%B0%EB%AF%B8%EB%84%90%EA%BE%B8%EB%AF%B8%EA%B8%B0-Oh-my-zsh-%ED%85%8C%EB%A7%88-%EA%B7%B8-%EB%B0%96%EC%97%90-%EC%B6%94%EA%B0%80-%EC%84%A4%EC%A0%95MacOS) 에서 확인

---



## 추가 기능

### (1) Terminal 'Last login' sign 제거하기

- Terminal root 에서 `touch .hushlogin` 파일 생성 후 재시작

### (2) Theme 설정 시 좋은 점

- Mac Terminal 기본 화면에서는 `git` 사용 시 `master` 표시가 확인되지 않는데 theme를 적용하면 확인 가능

### (3) oh-my-zsh 업데이트

```sh
$ omz update
```









