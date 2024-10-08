# SocialMetricsDjango

## APIs
### Twitter
#### Response
```json
{
  "status": int,
  "cache_response": bool,
  "cache_date": "str | %Y-%m-%d",
  "result": {
    "profile": {
      "image": " str | http:...",
      "name": "str",
      "username": "str",
      "id": "str",
      "bio": "str",
      "location": "str",
      "website": "str",
      "joined": " str | 2008-12-18T04:01:00",
      "stats": {
        "tweets": int,
        "following": int,
        "followers": int,
        "likes": int,
        "media": int,
        "avgRetweets": int,
        "avgLikes": int,
        "avgComments": int,
        "avgQuotes": int
      }
    },
    "tweets": [
      {
        "user": {
          "name": "str",
          "username": "str",
          "profile_id": "str",
          "avatar": "str | https:..."
        },
        "url": "str | https:...",
        "text": "str",
        "picture": "str | https:...",
        "video": [],
        "statistics": {
          "comments": int,
          "retweets": int,
          "quotes": int,
          "likes": int
        },
        "datetime": " str | 2024-09-05T17:17:00+00:00"
      },
    ]
}
```
#### History == True
```json
{
  "status": int,
  "user": "str",
  "result": [
    {
      "date": "date | 2024-08-26",
      "stats": {
        "tweets": int,
        "following": int,
        "followers": int,
        "likes": int,
        "media": int,
        "avgRetweets": int,
        "avgLikes": int,
        "avgComments": int,
        "avgQuotes": int
      }
    },
  ]
}
```
