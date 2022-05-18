# browserslist-config

A common browser list config for Chinese Desktop/Mobile using https://github.com/browserslist/browserslist.

[Environments](https://github.com/browserslist/browserslist#configuring-for-different-environments) for `production`.

**Desktop:**

File: `desktop.browserslistrc`

Main principle: `> 0.1% in CN and last 5 years, IE not dead, not ${Mobile}`

**Desktop Modern:**

File: `desktop-modern.browserslistrc`

Main principle: `> 0.1% in CN and last 3 years, not ${Mobile}`

**Mobile:**

File: `mobile.browserslistrc`

Main principle: `> 0.1% in CN and last 5 years, not ${Desktop}`

**Usual:**

File: `usual.browserslistrc`

Main principle: `> 0.1% in CN and last 5 years, IE not dead`

## Usage

Copy target file to your project `.browserslistrc`.

## Best Practices

- Queries order:

  1. `wide or + and`
  2. `specific versions`
  3. `not`

- `defaults` may not be for your project.

  Specify specific information for your query, such as `country`, `last versions`, `last years`.

  Sepcify not target platform information for your query, such as `not ie < 11`, `not ${Mobile}`, `not ${Desktop}`.

- Be dynamic

  Time is passing by every day. So `last 3 years` is better than `chrome >= 75`.

## Development

`BROWSERSLIST_CONFIG=desktop.browserslistrc npx browserslist@latest`

<details>
  <summary>result at 2022-05-18:</summary>
  <p>
    chrome 100
    chrome 99
    chrome 98
    chrome 97
    chrome 96
    chrome 95
    chrome 92
    chrome 90
    chrome 87
    chrome 86
    chrome 84
    chrome 83
    chrome 81
    chrome 80
    chrome 79
    chrome 78
    chrome 77
    chrome 75
    chrome 74
    chrome 72
    chrome 70
    chrome 69
    chrome 62
    edge 100
    edge 99
    edge 18
    firefox 99
    firefox 98
    firefox 91
    ie 11
    safari 15.4
    safari 14.1
    safari 14
    safari 13.1
  </p>
</details>
<br>

`BROWSERSLIST_CONFIG=desktop-modern.browserslistrc npx browserslist@latest`

<details>
  <summary>result at 2022-05-18:</summary>
  <p>
    chrome 100
    chrome 99
    chrome 98
    chrome 97
    chrome 96
    chrome 95
    chrome 92
    chrome 90
    chrome 87
    chrome 86
    chrome 84
    chrome 83
    chrome 81
    chrome 80
    chrome 79
    chrome 78
    chrome 77
    chrome 75
    edge 100
    edge 99
    firefox 99
    firefox 98
    firefox 91
    safari 15.4
    safari 14.1
    safari 14
    safari 13.1
  </p>
</details>
<br>

`BROWSERSLIST_CONFIG=mobile.browserslistrc npx browserslist@latest`

<details>
  <summary>result at 2022-05-18:</summary>
  <p>
    and_chr 101
    and_ff 100
    and_qq 10.4
    ios_saf 15.4
    ios_saf 15.2-15.3
    ios_saf 15.0-15.1
    ios_saf 14.5-14.8
    ios_saf 14.0-14.4
    ios_saf 13.4-13.7
    ios_saf 13.3
    ios_saf 12.2-12.5
    ios_saf 12.0-12.1
    ios_saf 11.0-11.2
    samsung 16.0
    samsung 14.0
    samsung 11.1-11.2
  </p>
</details>
<br>

`BROWSERSLIST_CONFIG=usual.browserslistrc npx browserslist@latest`

<details>
  <summary>result at 2022-05-18:</summary>
  <p>
    and_chr 101
    and_ff 100
    and_qq 10.4
    chrome 100
    chrome 99
    chrome 98
    chrome 97
    chrome 96
    chrome 95
    chrome 92
    chrome 90
    chrome 87
    chrome 86
    chrome 84
    chrome 83
    chrome 81
    chrome 80
    chrome 79
    chrome 78
    chrome 77
    chrome 75
    chrome 74
    chrome 72
    chrome 70
    chrome 69
    chrome 62
    edge 100
    edge 99
    edge 18
    firefox 99
    firefox 98
    firefox 91
    ie 11
    ios_saf 15.4
    ios_saf 15.2-15.3
    ios_saf 15.0-15.1
    ios_saf 14.5-14.8
    ios_saf 14.0-14.4
    ios_saf 13.4-13.7
    ios_saf 13.3
    ios_saf 12.2-12.5
    ios_saf 12.0-12.1
    ios_saf 11.0-11.2
    safari 15.4
    safari 14.1
    safari 14
    safari 13.1
    samsung 16.0
    samsung 14.0
    samsung 11.1-11.2
  </p>
</details>
