## head와 head 직전까지의 차분 test.zip으로 압축
git archive -o test.zip HEAD $(git diff --name-only HEAD^)
## tag1과 tag2의 차분 archive.zip으로 압축
git archive -o archive.zip HEAD $(git diff tag1 tag2)
## git 리포지토리 initial pull
git init<br>
git remote add origin https://github.com/kimhyunsuk/codeReference.git<br>
git branch --set-upstream-to=origin/master master<br>
git pull<br>
git pull --allow-unrelated-histories<br>
## git log ui 형태로 보기
gitk --all
