<h1> Hello Everyone <img src = "https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width = 30px> </h1>
<p align='center'></p>

<img width="55%" align="right" alt="Github" src="https://raw.githubusercontent.com/onimur/.github/master/.resources/git-header.svg" />

```YAML
name: AbhigyanTrips CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: '3.x'

      - name: Install dependencies
        run: |
          python -m pip install --upgrade pip

      - name: Run AbhigyanTrips Class
        run: |
          echo "Creating class instance..."
          python -c "
class AbhigyanTrips():
  def __init__(self):
    self.name = 'Abhigyan Tripathi'
    self.username = 'abhigyantrips'
    self.location = 'Mumbai, India'
    self.twitter = '@abhigyantrips'
    self.web = 'https://abhigyantrips.dev'
  def __str__(self):
    return self.name
```

<!--
**SmileDemon91/SmileDemon91** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on Banco Santander...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
