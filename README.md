Certainly! Below are the deployment steps for both Red Hat-based (such as CentOS) and Debian-based (such as Ubuntu) operating systems:

### Red Hat-based (e.g., CentOS) OS:

1. **Update Packages**: Ensure all packages are up to date by running the following command:
    ```bash
    yum update -y
    ```

2. **Install Git**: If Git is not installed, install it using the following command:
    ```bash
    yum install git
    ```

3. **Install httpd**: Install the Apache HTTP Server (httpd) using the following command:
    ```bash
    yum install httpd -y
    ```

4. **Clone the Repository**: Clone the GitHub repository containing your application.
    ```bash
    git clone https://github.com/saurabhkav03/deploy_app_using_httpd.git
    ```

5. **Navigate to the App Directory**: Change directory to the cloned repository.
    ```bash
    cd deploy_app_using_httpd/
    ```

6. **Copy App Files to httpd Directory**: Copy the application files to the httpd directory.
    ```bash
    cp -r ~/deploy_app_using_httpd/* /var/www/html/
    ```

7. **Start httpd Service**: Start the httpd service.
    ```bash
    systemctl start httpd
    ```

8. **Verify httpd Service**: Check the status of the httpd service to ensure it's running.
    ```bash
    systemctl status httpd
    ```

### Debian-based (e.g., Ubuntu) OS:

1. **Update Packages**: Ensure all packages are up to date by running the following command:
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```

2. **Install Git**: If Git is not installed, install it using the following command:
    ```bash
    sudo apt install git -y
    ```

3. **Install httpd**: Install the Apache HTTP Server (httpd) using the following command:
    ```bash
    sudo apt install apache2 -y
    ```

4. **Clone the Repository**: Clone the GitHub repository containing your application.
    ```bash
    git clone https://github.com/saurabhkav03/deploy_app_using_httpd.git
    ```

5. **Navigate to the App Directory**: Change directory to the cloned repository.
    ```bash
    cd deploy_app_using_httpd/
    ```

6. **Copy App Files to httpd Directory**: Copy the application files to the httpd directory.
    ```bash
    sudo cp -r ~/deploy_app_using_httpd/* /var/www/html/
    ```

7. **Start httpd Service**: Start the httpd service.
    ```bash
    sudo systemctl start apache2
    ```

8. **Verify httpd Service**: Check the status of the httpd service to ensure it's running.
    ```bash
    sudo systemctl status apache2
    ```

### Additional Information
- **Access the Application**: Open a web browser and navigate to the public IP address or domain name of your server to access the deployed application.
- **Customizing the App**: Modify the `index.html` file in the `deploy_app_using_httpd` directory to customize the content of your application.
- **Troubleshooting**: If you encounter any issues during the deployment process, refer to the logs or consult the documentation for httpd and your specific operating system.

