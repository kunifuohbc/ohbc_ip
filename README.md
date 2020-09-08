整数線形計画問題(Integer programming problem)を用いた優先業務選択システム
==============================

## Target

災害時における優先業務の選定を整数線形計画問題によってモデル化し，その最適値を算出する．

## Project Organization

    .
    ├── README.md          <- プロジェクトの全体像
    ├── model              <- 定式化に関するプログラム
    │   ├── .py
    │   └── .py    
    └── main.py            <- システムのメインプログラム

## Usage

### Step1

[Docker](https://www.docker.com/) で環境を作成します．事前に[公式ドキュメント](https://docs.docker.com/)を参照しローカル環境にDockerを導入してください．以下はDockerがインストールされており，DockerHubのアカウントを持っていることを想定しています．

### Step2

```shell
git clone git@github.com:kunifuohbc/ohbc_ip.git
```

### Step3

main.pyのあるディレクトリに移動し，使いたいデータをdata.xmlとしてそのディレクトリにおいて下さい．

### Step4

```shell
docker pull kunifuohbc/ohbc_ip
docker run -v $(pwd):/work kunifuohbc/ohbc_ip
```

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)


