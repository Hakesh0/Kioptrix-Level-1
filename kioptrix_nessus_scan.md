
# Kioptrix Level 1 - Nessus Vulnerability Scan

## Installing Nessus

1. Download the Nessus Debian package from the official website.
2. Open a terminal and navigate to the directory where the package is downloaded.
3. Install Nessus using the following command:
   ```bash
   sudo dpkg -i Nessus-10.7.2-debian10_amd64.deb
   ```

## Starting Nessus Scanner

1. Start the Nessus Scanner service by running the following command:
   ```bash
   sudo /bin/systemctl start nessusd.service
   ```

## Configuring Nessus Scanner

1. Open a web browser and go to https://kali:8834/ (replace "kali" with your Kali Linux hostname or IP address).
2. Follow the on-screen instructions to configure your Nessus Scanner.
3. Create a Nessus account or log in with your existing account.
4. After logging in, you will be directed to the Nessus Scanner dashboard.

## Performing a Vulnerability Scan

1. Click on "New Scan" in the Nessus Scanner dashboard.
2. Choose "Basic Scan" as the scan type.
3. Enter the IP address of the Kioptrix machine (e.g., 192.168.30.128) as the target for the scan.
4. Click "Scan" to start the vulnerability scan.

## Viewing Scan Results

1. After the scan completes, you will see a list of vulnerabilities found on the Kioptrix machine.
2. Cross-check the vulnerabilities with Google or other sources for reference and further research.

