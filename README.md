# OWASP-Dependency-Check

OWASP Dependency Check Installation and Running with a Node.js Project

1. Download the Latest CLI Version:

First, visit the [OWASP Dependency Check page](https://owasp.org/www-project-dependency-check/) to learn more about the project. To install the Dependency Check CLI, follow these steps:

# Create a directory for OWASP Dependency Check
mkdir owasp
cd owasp

# Download the latest release of Dependency Check
wget https://github.com/jeremylong/DependencyCheck/releases/download/v10.0.2/dependency-check-10.0.2-release.zip

# Unzip the downloaded file
unzip dependency-check-10.0.2-release.zip

2. Verify Installation:

Navigate to the bin directory of the unzipped Dependency Check folder to verify the installation:

cd /home/owasp/dependency-check/bin

# Verify using the shell script
./dependency-check.sh --version

3. Run a Scan on Your Node.js Project:

To scan your Node.js project for vulnerabilities, use the following steps:

# Navigate to your project directory
cd /home/project-folder

# Run the Dependency Check scan
/home/owasp/dependency-check/bin/dependency-check.sh --project user --out . --scan .

4. Review the Scan Report:

Once the scan is complete, a file named dependency-check-report.html will be created in your project directory. You can open this file in your web browser to review any detected vulnerabilities.
