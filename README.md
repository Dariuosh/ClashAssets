# ClashAssets

rule-providers:
  ir-bank:
    behavior: "domain" # domain, ipcidr or classical (premium core only)
    type: http
    url: "https://cdn.jsdelivr.net/gh/dariuosh/clashassets@master/Data/ir-bank.yaml"
    interval: 10
    path: /ir-bank.yaml
  ir-bourse:
    behavior: "domain" # domain, ipcidr or classical (premium core only)
    type: http
    url: "https://cdn.jsdelivr.net/gh/dariuosh/clashassets@master/Data/ir-bourse.yaml"
    interval: 10
    path: /ir-bourse.yaml
    
    
    
rules:

  - RULE-SET,ir-bank,DIRECT
  - RULE-SET,ir-bourse,DIRECT
  - GEOIP,IR,DIRECT
