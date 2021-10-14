# Usage

Recommended to create a class or a json file to storage all your twitter developer information
note: sometime you only need the bearer token if only getting users tweets and others stuffs.

## Example
``` python
class twitter:
    key='twitter-developer-key-here'
    secretKey='twitter-developer-secret-key-here'
    token='twitter-developer-token-code-here'
    secretToken='twitter-developer-secret-token-code-here'
    bearerToken='twitter-developer-bearer-token-here'
```

# Initialize module
``` python
tp = TwitterPlus(twitter.key,twitter.secretKey,twitter.token,twitter.secretToken,twitter.bearerToken)
```

# Get user id
``` python
userId = tp.getUserId('elonmusk')
print(userId)
```

# Get user tweets
max_results is between 5-200
``` python
userTweets = tp.timeline('elonmusk',max_results=20)
print(userTweets)
```