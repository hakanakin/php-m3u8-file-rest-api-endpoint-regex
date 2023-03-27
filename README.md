# PHP code for M3U file REST API endpoint

This PHP code creates a REST API endpoint that returns JSON data from an M3U file based on a GET request that searches for a given string in the `name` field.

## Usage

1. Save the PHP code as a file on your server (e.g. `api.php`).
2. Edit the `$m3u_file_path` variable to point to the location of your M3U file.
3. Call the endpoint using a URL with the search string as a query parameter, e.g. `http://example.com/api.php?search=bein`.
4. The endpoint will return a JSON object that contains the `name` and `link` fields for all entries in the M3U file that match the search string.

## Dependencies

This code has no external dependencies.


