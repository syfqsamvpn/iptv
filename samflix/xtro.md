## Usage

Run the script from the command line with the required arguments.

```bash
python main.py [OPTIONS]
```

### Arguments

| Short Option | Long Option        | Type   | Default | Description                                     |
|--------------|--------------------|--------|---------|-------------------------------------------------|
| `-u`         | `--url`           | String | None    | The URL to be processed.                       |
| `-i`         | `--input`         | String | None    | The input to be processed.                     |
| `-s`         | `--search_keyword`| String | None    | Search keyword to filter or search content.    |
| `-x`         | `--limit_series`  | Int    | 100     | Limit the episodes per series (default: 100).  |
| `-l`         | `--limit_scrap`   | Int    | 25      | Limit the scraping results (default: 25).      |
| `-n`         | `--notification_update` | String | `y`   | Enable/disable notifications (`y` or `n`).     |

### Examples

#### Process a URL

```bash
python main.py --url "http://example.com"
```

#### Provide input to be processed

```bash
python main.py --input "some_input_value"
```

#### Search using a keyword

```bash
python main.py --search_keyword "example_keyword"
```

#### Customize limits for series and scraping

```bash
python main.py --limit_series 50 --limit_scrap 10
```

#### Disable notifications

```bash
python main.py --notification_update n
```

### Notes

- You can use short (`-u`) or long (`--url`) options interchangeably.
- Multiple arguments can be combined in a single command.
- Arguments without a specified default value are optional, but the script's functionality may vary based on which arguments are provided.
