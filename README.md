# Dummy JSON Data Repository

This repository serves as a storage for JSON files used as dummy fetch data for various projects. It supports pagination by using the file naming convention to indicate the page number and page size.


Files are named following this format:

```
<file_name>_<page_number>_<page_size>_<other_params>.json
```

### Example:

- `product_5_10.json` → Fetches **products** on **page 5** with **page size = 10**.
- `user_2_20.json` → Fetches **users** on **page 2** with **page size = 20**.

## Usage

You can fetch data in your project by requesting the corresponding JSON file based on the required page and size.

### Example Fetch Request:

```javascript
fetch('https://raw.githubusercontent.com/your-username/your-repo/main/product_5_10.json')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error fetching data:', error));
```

## Contribution

If you want to add or update data, please follow the naming convention and ensure JSON files are properly formatted.

## License

This repository is open for public use. Feel free to use it for testing and development purposes!

