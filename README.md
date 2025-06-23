![](banner.jpg)

# openwhenready

## Purpose

This script polls a specified URL until it returns a successful HTTP status code (2xx or 3xx). Once a successful response is received, it opens the URL in the default browser or Google Chrome (optional). It times out after 10 minutes if the URL never becomes ready.

## Usage

```bash
openwhenready [--chrome] <url>
```

*   `<url>`: The URL to poll.
*   `[--chrome]`: An optional flag to force opening the URL in Google Chrome. If not specified, the default browser will be used.

## Examples

1.  Open `https://example.com` in the default browser when it's ready:

    ```bash
    openwhenready https://example.com
    ```

2.  Open `https://example.com` in Google Chrome when it's ready:

    ```bash
    openwhenready --chrome https://example.com
    ```

## Installation

1.  Save the script to a file named `openwhenready`.
2.  Make the script executable:

    ```bash
    chmod +x openwhenready
    ```

3.  (Optional) Move the script to a directory in your `PATH` (e.g., `/usr/local/bin`) to make it accessible from anywhere:

    ```bash
    sudo mv openwhenready /usr/local/bin
    ```