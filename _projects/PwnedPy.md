---
title: "PwnedPy"
excerpt: "A Python Wraper/Module for the Have I been Pwned API"
sidebar:
  - title: "Language(s) Used"
    text: "Python"
  - title: "License"
    text: "MIT"
  - title: "Requirements"
    text: "Requests, JSON"
  - title: "Created On"
    text: "05-05-2019"
---

> A Python Wraper/Module for the Have I been Pwned API

![PyPI - License](https://img.shields.io/pypi/l/PwnedPy.svg) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/cbe32a93922141a693b9679229ffcfbd)](https://www.codacy.com/app/navanchauhan/PwnedPy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=navanchauhan/PwnedPy&amp;utm_campaign=Badge_Grade)

### Installation
```
pip3 install PwnedPy
```
### Initialisation
```
import PwnedPy
```
or
```
import PwnedPy as pp
```
### Functions

| Function | Optional Values | Required Values | Example | Output |
|----------|-----------------|--------|---------|-----------|
| getAllBreaches | domain | None | breaches = PwnedPy.getAllBreaches(domain="adobe.com")| JSON |
| getBreaches | Truncated and Unverified | account | breaches = pp.getBreaches("navanchauhan@gmail.com", Truncated=True, Unverified=True) | JSON |
| getBreachesByDomain | Truncated and Unverified | account and domain | breaches = PwnedPy.getBreachesByDomain("navanchauhan@gmail.com", domain="dubsmash.com") | JSON |
| getPastes | None | account | breaches = pp.getPastes("navanchauhan@gmail.com") | JSON |
