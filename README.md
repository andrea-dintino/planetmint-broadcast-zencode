
![Zenswarm](https://github.com/dyne/zenswarm/blob/main/docs/zenswarm.svg)



<h1 align="center">
Planetmint Broadcast Zencode
  </br>
  <sub>Execute Zenroom SC in Planetmint monitoring</sub>
</h1>

<p align="center">
  <a href="https://dyne.org">
    <img src="https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%9D%A4%20by-Dyne.org-blue.svg" alt="Dyne.org">
  </a>
</p>

<br><br>

<h4 align="center">
  <a href="#-install">💾 Install</a>
  <span> • </span>
  <a href="#-quick-start">🎮 Quick start</a>
  <span> • </span>
  <a href="#-configuration">🔧 Configuration</a>
  <span> • </span>
  <a href="#-testing">📋 Testing</a>
  <span> • </span>
  <a href="#-troubleshooting--debugging">🐛 Troubleshooting & debugging</a>
  <span> • </span>
  <a href="#-acknowledgements">😍 Acknowledgements</a>
  <span> • </span>
  <a href="#-links">🌐 Links</a>
  <span> • </span>
  <a href="#-contributing">👤 Contributing</a>
  <span> • </span>
  <a href="#-license">💼 License</a>
</h4>


A python script to execute a <a href="https://dev.zenroom.org">Zenroom</a> smart contract in <a href="https://planetmint.io">Planetmint</a>.  

The script performs a POST to a Planetmint node, which is executed on chain. Upon successful execution, Planetmint returns a txId. Data passed to Planetmint is:

* A smart contract written in Zencode 
* Input for the smart contract
* ED259 public key of the actor executing the smart contract

Example

```bash
curl -X POST localhost:5000/broadcast --data-urlencode "data@data.json" --data-urlencode "keys@keys.json" --data-urlencode "script@script.zen" --data-urlencode "asset@asset.json" --data-urlencode "ed_public_key=5Uv4KLinWJpKFagfab9r3P9jMRJhWMZv3CgRdBZZ4vvb" --data-urlencode "metadata@metadata.json"
```

<details id="toc">
 <summary><strong>🚩 Table of Contents</strong> (click to expand)</summary>

* [Install](#-install)
* [Quick start](#-quick-start)
* [Links](#-links)
* [Contributing](#-contributing)
* [License](#-license)
</details>

***
## 💾 Install
```
pnpm install
pnpm run build
pnpm run start
```


***
## 🎮 Quick start

```pnpm run dev```


***

**[🔝 back to top](#toc)**

***
## 😍 Acknowledgements

[![software by Dyne.org](https://files.dyne.org/software_by_dyne.png)](http://www.dyne.org)

Copyleft (ɔ) 2021 by [Dyne.org](https://www.dyne.org) foundation, Amsterdam

Designed, written and maintained by Puria Nafisi Azizi.

Special thanks to Mr. W. White for his special contributions.

**[🔝 back to top](#toc)**

***
## 🌐 Links

https://github.com/dyne/zenswarm
https://dyne.org/

**[🔝 back to top](#toc)**

***
## 👤 Contributing

Please first take a look at the [Dyne.org - Contributor License Agreement](CONTRIBUTING.md) then

1.  🔀 [FORK IT](../../fork)
2.  Create your feature branch `git checkout -b feature/branch`
3.  Commit your changes `git commit -am 'Add some fooBar'`
4.  Push to the branch `git push origin feature/branch`
5.  Create a new Pull Request
6.  🙏 Thank you


**[🔝 back to top](#toc)**

***
## 💼 License
    Planetmint Broadcast Zencode - {tagline}
    Copyleft (ɔ) 2021 Dyne.org foundation, Amsterdam

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

**[🔝 back to top](#toc)**
