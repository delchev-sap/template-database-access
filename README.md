# Template - Database Access

[![Eclipse License](http://img.shields.io/badge/license-Eclipse-brightgreen.svg)](LICENSE)
[![GitHub contributors](https://img.shields.io/github/contributors/dirigiblelabs/template-v3-database-access.svg)](https://github.com/dirigiblelabs/template-v3-database-access/graphs/contributors)


## Overview

Simple "Database Access" JavaScript service
```javascript
var query = require('db/v3/query');
var response = require('http/v3/response');


var sql = 'select * from DIRIGIBLE_EXTENSIONS where EXTENSION_EXTENSIONPOINT_NAME = ?';

var resultset = query.execute(sql, ['ide-template']);

response.println(JSON.stringify(resultset));

response.flush();
response.close();
```


## License

This project is copyrighted by [SAP SE](http://www.sap.com/) and is available under the [Eclipse Public License v 1.0](https://www.eclipse.org/legal/epl-v10.html). See [LICENSE](LICENSE) and [NOTICE.txt](NOTICE.txt) for further details.
