# ADM FINDER

## Overview
ADM FINDER is an advanced admin page scanner designed to identify administrative login portals on websites efficiently. This tool utilizes multi-threading, custom request headers, and response validation mechanisms to enhance detection accuracy while minimizing false positives.

## Features
- **Multi-threaded Scanning:** Uses `ThreadPoolExecutor` to speed up the scanning process.
- **Customizable Request Methods:** Supports GET, POST, and HEAD requests for flexible scanning.
- **Automatic URL Validation:** Ensures proper URL formatting and corrects missing protocols (http/https).
- **Session Management:** Implements retry mechanisms with backoff strategies to handle network failures.
- **Advanced Response Handling:** Detects HTTP status codes, redirects, and keyword matches in responses.
- **Captcha Detection:** Warns if a captcha is present, suggesting a need for adjustments.
- **HTML Report Generation:** Outputs scan results in a structured, user-friendly HTML report with interactive design.
- **Rich Console UI:** Uses `rich` library for an improved visual experience, including banners and progress bars.

## Dependencies
Ensure you have the following Python packages installed:
```sh
pip install requests rich
```

## Usage
Run the script and specify the target website:
```sh
python adm_finder.py -u example.com
```

### Options:
- `-u, --url`: Target URL to scan.
- `-k, --keyword`: Keyword to match in responses.
- `-m, --method`: Request method (default: GET).
- `-t, --threads`: Number of threads to use (default: 10).

## Example
```sh
python adm_finder.py -u example.com -k "admin" -t 20
```

## Report
After scanning, results are saved in an HTML report named `scan_report_<timestamp>.html` with details of each detected admin page.

## Contact
- **Telegram:** [@KALOSHA319](https://t.me/KALOSHA319)
- **Facebook:** [KALEGY3199](https://www.facebook.com/KALEGY3199/)

