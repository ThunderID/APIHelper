# Thunder API Helper

Package contain engine to help basic API Post & Request.

# Require
Guzzlehttp/guzzle": "~5.3"

# Installation

composer.json:
```
	"thunderid/APIHelper": "dev-master"
```

run
```
	composer update
```

```
	composer dump-autoload
```

# Usage

service provider
```
'ThunderID\APIHelper\ThunderAPIHelperServiceProvider::class'
```

Aliases

1. API connector
desc : to comunicate (post/get) data (to/from) api
```
'API' => ThunderID\APIHelper\API\APIData::class,
```
