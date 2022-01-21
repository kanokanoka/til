# APIによる脆弱性情報取得

ここがわかりやすい

NVD公開のREST APIを用いて脆弱性情報を取得する  
https://qiita.com/riikunn_ryo/items/97e385ed0a78dc28534f

CVEとかCWEをNVDが公開するAPIを用いて取得している。

例えばこう

    curl https://services.nvd.nist.gov/rest/json/cve/1.0/cve-2019-7609|jq .

jsonで帰ってくる

    {
      "resultsPerPage": 1,
      "startIndex": 0,
      "totalResults": 1,
      "result": {
        "CVE_data_type": "CVE",
        "CVE_data_format": "MITRE",
        "CVE_data_version": "4.0",
        "CVE_data_timestamp": "2022-01-21T09:48Z",
        "CVE_Items": [
          {
     (略)
