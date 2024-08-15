# 0x03. Log Parsing

This project focuses on developing a script to parse logs, extract relevant data, and compute metrics such as file size and HTTP status codes from stdin input.

## Tasks :page_with_curl:

* **0. Log parsing**
  * **[0-stats.py](./0-stats.py):** This script reads lines from standard input (stdin), parses them, and computes the following metrics:
    - **Total file size:** Cumulative sum of file sizes from the parsed logs.
    - **Status codes:** Count of occurrences for each HTTP status code (200, 301, 400, 401, 403, 404, 405, 500).

    The script outputs these metrics every 10 lines and upon receiving a keyboard interruption (CTRL + C).

  * **Usage:**
    ```bash
    ./0-generator.py | ./0-stats.py
    ```

    **Example Output:**
    ```
    File size: 5213
    200: 2
    401: 1
    403: 2
    404: 1
    405: 1
    500: 3
    ```

  * **Input Format:**
    ```
    <IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>
    ```
    - The script will skip any lines that do not match this format.

  * **Annotations:**
    - The status codes are printed in ascending order.
    - If a status code doesn’t appear or is not an integer, it will not be included in the output.
