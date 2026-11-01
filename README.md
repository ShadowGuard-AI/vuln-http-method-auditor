# vuln-HTTP-Method-Auditor
Audits a website's allowed HTTP methods for each endpoint, highlighting potential vulnerabilities arising from allowing unintended methods like PUT, DELETE, or TRACE. A method counts as allowed only on a 2xx response to that method. A 301, 302, 303, 307, or 308 response is reported as the value "redirect" rather than as allowed, and redirects are not followed. Endpoints must be listed explicitly with -e. - Focused on Assess vulnerabilities in web applications by performing scans and providing detailed reports

## Install
`git clone https://github.com/ShadowStrikeHQ/vuln-http-method-auditor`

## Usage
`./vuln-http-method-auditor [params]`

## Parameters
- `-h`: Show help message and exit
- `-u`: The target URL to audit.
- `-e`: Specific endpoints to test. If not provided, attempts to test all discovered endpoints.
- `-m`: No description provided
- `-o`: No description provided
- `-v` / `--verbose`: Enable verbose output, including the per method status codes.
- `--user-agent`: Custom User-Agent string.
- `--timeout`: Request timeout in seconds.
- `--ignore-ssl`: Ignore SSL certificate validation errors.

## License
Copyright (c) ShadowStrikeHQ
