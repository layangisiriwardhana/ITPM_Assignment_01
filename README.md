# Test Automation Project

This project combines Playwright for browser automation tests and a Python script for running test cases from an Excel file.

## Prerequisites

- Node.js (for Playwright)
- Python 3.x
- Playwright browsers installed

## Installation

1. Install Node.js dependencies:
   ```bash
   npm install
   ```

2. Install Playwright browsers:
   ```bash
   npx playwright install
   ```

3. Install Python dependencies (if any):
   ```bash
   pip install -r requirements.txt
   ```

## Running Tests

### Playwright Tests
Run the Playwright tests:
```bash
npx playwright test
```

Run specific test file:
```bash
npx playwright test tests/example.spec.js
```

### Python Test Automation Script
Run the Python script with Excel test cases:
```bash
python test_automation.py --excel "path/to/test_cases.xlsx" --url "https://example.com" --wait-ms 15000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1
```

Options:
- `--excel`: Path to the Excel file with test cases
- `--url`: Target URL for testing
- `--wait-ms`: Wait time in milliseconds
- `--type-delay-ms`: Delay between typing characters
- `--slow-mo-ms`: Slow motion delay for actions
- `--save-every`: Save frequency

## Configuration

- `playwright.config.js`: Playwright configuration
- `package.json`: Node.js dependencies

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make changes
4. Run tests
5. Submit a pull request