# 0x04. UTF-8 Validation

This project involves creating a method to validate if a given dataset represents a valid UTF-8 encoding. The goal is to understand how UTF-8 encoding works and apply that knowledge to validate the encoding in a dataset.

## Tasks :page_with_curl:

* **0. UTF-8 Validation**
  * **[0-validate_utf8.py](./0-validate_utf8.py):** Write a method `validUTF8(data)` that determines if a given dataset represents a valid UTF-8 encoding.

    * **Prototype:**
      ```python
      def validUTF8(data):
      ```

    * **Returns:**
      * `True` if `data` is a valid UTF-8 encoding.
      * `False` otherwise.

    * **Requirements:**
      * A character in UTF-8 can be 1 to 4 bytes long.
      * The dataset can contain multiple characters.
      * The data will be represented by a list of integers.
      * Each integer represents 1 byte of data, therefore you only need to handle the 8 least significant bits of each integer.

    * **Usage:**
      ```python
      validUTF8 = __import__('0-validate_utf8').validUTF8

      data = [65]
      print(validUTF8(data))  # Output: True

      data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
      print(validUTF8(data))  # Output: True

      data = [229, 65, 127, 256]
      print(validUTF8(data))  # Output: False
      ```

    * **Expected Output:**
      ```python
      True
      True
      False
      ```
