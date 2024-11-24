# Json module documentation

## JSON Handling Functions

This module contains two functions for saving and loading data in JSON format: `save_json` and `load_json`.

## `save_json(data: dict, file_path: str) -> None`

Saves a Python dictionary to a JSON file at the specified file path.

### Parameters:

-   **data** (`dict`): The dictionary (or any JSON serializable object) to save to a JSON file.
-   **file_path** (`str`): The path where the JSON file will be saved. This can be either a relative or absolute path.

### Returns:

-   **None**

### Example Usage:

```python
data = {"name": "Alice", "age": 25}
save_json(data, 'user_data.json')
```

### Notes:

-   The function will overwrite the file if it already exists.
-   The file is saved with an indentation of 2 spaces and with proper separators to improve readability.

---

## `load_json(file_path: str) -> dict | None`

Loads data from a JSON file into a Python dictionary.

### Parameters:

-   **file_path** (`str`): The path to the JSON file that should be loaded. This can be either a relative or absolute path.

### Returns:

-   **dict | None**: Returns the data as a Python dictionary if the file exists and is correctly formatted, or `None` if the file does not exist or is not valid JSON.

### Example Usage:

```python
data = load_json('user_data.json')
```

### Notes:

-   If the file does not exist or is not a valid JSON file, the function will return `None`.

---
