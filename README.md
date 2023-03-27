# PHP code for M3U file REST API endpoint

This PHP code creates a REST API endpoint that returns JSON data from an M3U file based on a GET request that searches for a given string in the `name` field.

## Usage

1. Save the PHP code as a file on your server (e.g. `api.php`).
2. Edit the `$m3u_file_path` variable to point to the location of your M3U file.
3. Call the endpoint using a URL with the search string as a query parameter, e.g. `http://example.com/api.php?search=bein`.
4. The endpoint will return a JSON object that contains the `name` and `link` fields for all entries in the M3U file that match the search string.

### JSON output

The endpoint returns a JSON object with the following structure:

{
"results": [
{
"name": "TR: CHANNEL NAME 1",
"link": "https://example.com:443/111111/11111/112180"
},
{
"name": "USA: CHANNEL NAME",
"link": "https://example.com:443/111111/11111/112180"
},
...
]
}


The `results` field contains an array of objects, each representing a single entry in the M3U file that matches the search string. Each object has a `name` field, which contains the name of the channel, and a `link` field, which contains the link to the channel's stream.

## Dependencies

This code has no external dependencies.

## License

This code is released under the MIT license. See the `LICENSE` file for more information.
