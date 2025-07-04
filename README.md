# リリースノート自動生成機能を利用してリリースを作成するアクション

## 使い方
```yaml
      - uses: daiichi-g/create-release-with-generated-notes@v1
        with:
          tag: 'v1.0.0'
```

## オプション
### 前回のリリースのタグを指定する場合
```yaml
      - uses: daiichi-g/create-release-with-generated-notes@v1
        with:
          tag: 'v1.0.0'
          previous-tag: 'v0.9.0'
```

### ドラフトとして作成する場合
```yaml
      - uses: daiichi-g/create-release-with-generated-notes@v1
        with:
          tag: 'v1.0.0'
          draft: true
```

### プレスリリースとして作成する場合
```yaml
      - uses: daiichi-g/create-release-with-generated-notes@v1
        with:
          tag: 'v1.0.0'
          prerelease: true
```



## パラメータ
| パラメータ名 | 必須 | 説明 |
|:---|:---:|:---|
| tag |必須 | リリースのタグ名 |
| previous-tag | | 前回のリリースのタグ名 |
| draft | | true: ドラフトとして作成する |
| prerelease | | true: プレスリリースとして作成する |
