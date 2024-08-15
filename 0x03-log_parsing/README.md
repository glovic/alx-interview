# 0x03. Log Parsing

This project involves creating a script to parse logs and compute metrics. The focus is on processing input lines, extracting relevant data, and outputting summary statistics based on status codes and file sizes.

## Tasks :page_with_curl:

* **0. Log parsing**
  * **Mandatory**
  * Write a script that reads stdin line by line and computes metrics:
    - **Input Format:** 
      ```
      <IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>
      ```
      - If the format is incorrect, the line must be skipped.
    - **Output:**
      - After every 10 lines and/or a keyboard interruption (CTRL + C), print the following statistics:
        - **Total file size:** 
          ```
          File size: <total size>
          ```
          - `<total size>` is the sum of all previous `<file size>` values.
        - **Number of lines by status code:** 
          ```
          <status code>: <number>
          ```
          - Possible status codes: `200, 301, 400, 401, 403, 404, 405, 500`.
          - If a status code doesn’t appear or is not an integer, don’t print anything for that status code.
          - Status codes should be printed in ascending order.

  * **Usage:**
    ```
    ./0-generator.py | ./0-stats.py 
    ```
    - This will run the generator script and pipe its output into your log parsing script.
  
  * **Annotations:**
    - The log generator script (`0-generator.py`) creates random logs for testing, while the log parsing script (`0-stats.py`) reads these logs and computes the required metrics.

  * **Example Output:**
    ```
    File size: 5213
    200: 2
    401: 1
    403: 2
    404: 1
    405: 1
    500: 3
    ```
