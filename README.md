# Ops-with-IaC
Cloud infrastructure operation using IaC.

## Install Terraform
https://developer.hashicorp.com/terraform/cli/install/apt

## Connect to Git
https://www.lainyzine.com/ko/article/summary-of-how-to-use-git-for-source-code-management/

### Install Git using apt-get
$ sudo apt-get update
$ sudo apt-get install git

## Install Atlantis
https://www.runatlantis.io/guide/testing-locally.html

### 최신버전 다운로드
https://github.com/runatlantis/atlantis/releases

참고(v0.22.2-linux_amd64)
https://github.com/runatlantis/atlantis/releases/download/v0.22.2/atlantis_linux_amd64.zip

### unzip
$ sudo apt install unzip
$ unzip [file name] -d .

### ngrok 다운로드 & 설치
https://ngrok.com/download

curl -s https://ngrok-agent.s3.amazonaws.com/ngrok.asc | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" | sudo tee /etc/apt/sources.list.d/ngrok.list && sudo apt update && sudo apt install ngrok


### ngrok 실행
ngrok http 4141

URL="https://{YOUR_HOSTNAME}.ngrok.io"

## Value

### webhook secret
0ltbcayimgd87x3dbg3i

### Private token
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

### run server
./atlantis server \
--atlantis-url="https://92e1-13-209-167-35.jp.ngrok.io" \
--gh-user="choihaemin" \
--gh-token="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" \
--gh-webhook-secret="0ltbcayimgd87x3dbg3i" \
--repo-allowlist="github.com/choihaemin/Ops-with-IaC"
