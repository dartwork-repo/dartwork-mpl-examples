# 저장소 설명

이 저장소는 `dartwork-mpl`을 깃 서브모듈로 포함합니다 (깃 저장소를 포함하는 깃 저장소 개념). 따라서 이 저장소에 있는
`./dartwork-mpl`의 수정 사항은 `dartwork-mpl`의 원격 저장소에 푸쉬할 수 있습니다. 

주의할 점은 이 저장소를 클론할 때 서브모듈까지 클론하기 위해서 아래와 같이 `--recursive` 옵션을 추가해야 합니다.

```
git clone --recursive https://github.com/dartwork-repo/dartwork-mpl-examples.git
```

라이브러리 설치는 아래와 같이 수정 가능한 버전으로 설치합니다.

```
pip install --editable ./dartwork-mpl
```

수정 가능한 버전으로 설치해야지만 `./dartwork-mpl`의 내용을 수정했을 때 설치된 `dartwork-mpl`
기능도 업데이트 됩니다. 그렇지 않으면 분리된 라이브러리 저장폴더에 `./dartwork-mpl` 내용이 카피되어 
설치되기 때문에 `./dartwork-mpl`의 변경 사항이 반영되지 않습니다.