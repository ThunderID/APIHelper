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
//continued

service provider
```
'ThunderID\ThunderOauthSQL\ThunderOauthSQLServiceProvider'
```

migration
```
php artisan migrate --path vendor/thunderid/thunderoauth-sql/src/migrations/
```

authorized engine
```
new ThunderID\ThunderOauthSQL\Authorizer(app('request'))
```

middleware oauth (kernel)
```
'oauth' 		=> ThunderID\ThunderOauthSQL\Middleware\OAuthMiddleware::class
```

middleware oauth (route group)
```
'middleware' => 'oauth'
```

middleware oauth scope (kernel)
```
'oauth-scope' 		=> ThunderID\ThunderOauthSQL\Middleware\OAuthScopeMiddleware::class
```

middleware oauth scope (route group)
```
'middleware' => 'oauth-scope:employee'
```
