# vscode-server-cfn

## AWS Cloudformation을 사용한 code-server 구축 CNF입니다.

Cloudformation Stack을 생성하실 때, 파라미터 값을 3개만 수정하시면 됩니다.
 - WebVscodeDomainName에 구매하신 도매인 이름을 넣어주세요.
 - WebVscodeEmail에 사용할 Email주소를 넣어주세요.
 - WebVscodeSSHKeyName에 만드신 ssh key 이름을 넣어주세요.

## 순서는 다음과 같습니다.

1. 도매인 구매.
2. cloudformation 배포
3. 배포 후 ec2 public ip 주소를 가지고 DNS A Record 생성.
4. ec2에 접속 후 `~/.start.sh` 실행

## Architecture
![code-server](https://user-images.githubusercontent.com/15880397/139571123-1bc2223a-d99c-4b42-a7ef-2f6f1eca06cc.png)
