# ktds

Kotlin TDS

# Configuration


Example campaign file

```
id: "campaign1"
offers:
  - id: "offer-firefox"
    matchers:
      userAgent:
        - "firefox.*"
      
    urls:
      - http://default1.test?sid=${sid}
      - http://default2.test?sid=${sid}

  - id: "offer1-cn"
    matchers:
      country:
        - "cn"

    urls:
      - http://default1.cn?sid=${sid}
      - http://default2.cn?sid=${sid}

  - id: "default"
    matchers:
    urls:
      - http://default2.default?sid=${sid}
      - http://default2.default?sid=${sid}

      
```

# Usage

./gradlew run