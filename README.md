# mal

`mal` is a command-line client for [MyAnimeList.net](http://myanimelist.net/). It uses the [official REST API](http://myanimelist.net/modules.php?go=api), so it shouldn't break in the near future.

## Requirements

- Python 3 or possibly Python 2.7 (untested)
- [requests](http://docs.python-requests.org/en/latest/index.html)


## Configuration

First, create `~/.myanimelist.ini` and fill it with your MAL account details:

```ini
[mal]
username = your_username
password = your_password
```

Yes, it's stored plain text, deal with it for now.


## Usage

Currently `mal` has rather limited functionality:

- Search your anime list with `mal [regex]`
- Increment the number of episodes watched with `mal inc [regex]`. If there are multiple matches, it prompts you to select which one. If incrementing from 0, it sets the anime status to "watching" and sets the start date to today. If incrementing to the total episode count, it sets the anime status to "completed" and sets the end date to today.

More should be coming eventually.
