# monorepo-smart-deploy-test
어케하지


1. 스크립트 짜서 change 찾아서 배포 스크립트 돌리기
  - `git diff origin/main...HEAD --name-only | grep ^서비스들/` 뭐 이런거 활용하면 되긴 할듯
2. change 를 똑똑하게 찾아줄 것 같은 lerne
  - `lerne run <blah> --since=origin/main` 이런거 가능한데 위에랑 뭐가 다른지 모르겠음
  - monorepo 관리가 좀 더 편하긴 할텐데... (각 service 의 script 실행 같은거) 근데 이 기능을 쓸지 모르겠음. 그전엔 이런거 없어도 잘살았음.
  - 근데 각 npm script 에 deploy 같은거 추가해서 lerne run deploy --since=origin/main 이렇게 돌리면 되긴 할듯. 근데 package manager script 에 deploy 가 있는게 맞나? 엄...
3. github action 에 on push main && path 조건 주면 알아서 안해주나?
  - 해준다. 굿. 근데 이거 deploy script 를 service 마다 만들어줘야하는... 단점이 있음
  - script template 화 할 수 있을것 같은디
