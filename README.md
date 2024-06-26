# 저장소 설명

이 저장소는 `dartwork-mpl`을 사용한 plot example에 관한 것입니다. 다음과 같은
커멘드로 dartwork-mpl을 설치하세요.

```bash
pip install git+https://github.com/dartwork-repo/dartwork-mpl
```















# 과거 설명 (사용하지 마세요)

이 저장소는 `dartwork-mpl`을 사용한 plot example에 관한 것입니다. 
이는 `dartwork-mpl`을 깃 서브모듈로 포함합니다.  
깃 서브모듈이란 하나의 깃 저장소 안에 다른 깃 저장소를 포함하는 개념입니다. 
따라서, 이 저장소 내의 `./dartwork-mpl`에서 발생한 변경 사항들은 `dartwork-mpl`의 remote repository로 push할 수 있습니다. 

example repository를 클론할 때는 서브모듈까지 함께 클론하기 위해 아래와 같이 --recursive 옵션을 사용해야 합니다:

```
git clone --recursive https://github.com/dartwork-repo/dartwork-mpl-examples.git
```

라이브러리 설치는 아래와 같이 --editable을 사용하여 수정 가능한 버전으로 설치합니다. 
수정 가능한 버전으로 설치해야지만 서브모듈 `./dartwork-mpl`의 수정이 오리지널 `dartwork-mpl` 에도 반영됩니다.  
만약 이렇게 설치하지 않을 경우, ./dartwork-mpl의 변경 사항이 별도의 라이브러리 폴더에 복사되어 설치되므로, 서브모듈로 작동하는 `./dartwork-mpl`에서의 변경 사항이 오리지널 repo인 `dartwork-mpl`에 반영되지 않습니다. 


```
pip install --editable ./dartwork-mpl
```
이 때 서브모듈 `dartwork-mpl`의 설치 경로는 dartwork-mpl-examples 폴더 내부로 설정되어서 nested library처럼 위치하도록 해야 합니다. 
VSCode 상에서 submodule을 의미하는 S 마크가 표시되어 있는지 확인합니다. 

remote repo에 있는 최신 버전의 `dartwork-mpl`을 설치하기 위해서는 `./dartwork-mpl`에 진입하여 `git pull`을 수행하면 됩니다. 
반대로 `./dartwork-mpl`의 내용을 원격 저장소에 올리기 위해서는 `git push`를 입력합니다. 
이러한 과정은 VSCode GUI에서도 수행할 수 있습니다.
