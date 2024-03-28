# Subdir - Subdomain Enumeration

Subdir is a Python script for enumerating subdomains using the SecurityTrails API. It allows users to quickly discover subdomains associated with a given domain by leveraging the SecurityTrails API.

## How to Run

1. **Prerequisites**: Ensure you have Python installed on your system.

2. **Permission and Installation**:
   
   - Make the script executable:
     ```
     chmod +x subdir
     ```

   - Move the script to the bin directory (optional, for global usage):
     ```
     sudo mv subdir /usr/local/bin/subdir
     ```

3. **Usage**:
   
   - To enumerate subdomains for a domain and save them to a file:
     ```
     subdir spaceX.com subdomains.txt
     ```

4. **Configuration Directory**:

   - Upon running the script, a folder named `.subdirconfig` will be created in your home directory. This folder contains a file named `config` where users can store their SecurityTrails API key for authentication.

## Note

- For authentication, users need to provide their SecurityTrails API key. The key can be obtained from the SecurityTrails website.
- The script periodically checks the usage of the SecurityTrails API and displays the usage information after every 5 hours.
