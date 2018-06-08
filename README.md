# pg-concat
[![Tymly Package](https://img.shields.io/badge/tymly-package-blue.svg)](https://tymly.io/) [![npm (scoped)](https://img.shields.io/npm/v/@wmfs/pg-concat.svg)](https://www.npmjs.com/package/@wmfs/pg-concat) [![Build Status](https://travis-ci.org/wmfs/pg-concat.svg?branch=master)](https://travis-ci.org/wmfs/pg-concat) [![codecov](https://codecov.io/gh/wmfs/pg-concat/branch/master/graph/badge.svg)](https://codecov.io/gh/wmfs/pg-concat) [![CodeFactor](https://www.codefactor.io/repository/github/wmfs/pg-concat/badge)](https://www.codefactor.io/repository/github/wmfs/pg-concat) [![Dependabot badge](https://img.shields.io/badge/Dependabot-active-brightgreen.svg)](https://dependabot.com/) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/wmfs/tymly/blob/master/packages/pg-concat/LICENSE)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwmfs%2Fpg-concat.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwmfs%2Fpg-concat?ref=badge_shield)




> Takes an array of parts and returns the necessary PostgreSQL expression to concatenate them.

## Usage

```
const pgConcat = require('pg-concat')

const concatString = pgConcat(
    [
        { columnName: 'incident_no' },
        '/',
        { columnName: 'year', default: 1900 },
    ]
)

// concatString = 'incident_no||'/'||COALESCE(year, 1900)'
```

## <a name="install"></a>Install
```bash
$ npm install pg-concat --save
```

## <a name="license"></a>License
[MIT](https://github.com/wmfs/pg-concat/blob/master/LICENSE)


[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwmfs%2Fpg-concat.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwmfs%2Fpg-concat?ref=badge_large)