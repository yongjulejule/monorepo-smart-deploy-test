# monorepo-smart-deploy-test
어케하지


1. 스크립트 짜서 change 찾아서 배포 스크립트 돌리기
  - `git diff origin/main...HEAD --name-only | grep ^서비스들/` 뭐 이런거 활용하면 되긴 할듯
2. change 를 똑똑하게 찾아줄 것 같은 lerne
  - `lerne run <blah> --since=origin/main` 이런거 가능한데 위에랑 뭐가 다른지 모르겠음
  - monorepo 관리가 좀 더 편하긴 할텐데... (각 service 의 script 실행 같은거) 근데 이 기능을 쓸지 모르겠음. 그전엔 이런거 없어도 잘살았음.
3. github action 에 on push main && path 조건 주면 알아서 안해주나? 
