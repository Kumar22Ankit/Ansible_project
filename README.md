<h1><u></u>EC2 Apache Setup with Ansible</h1>

<h3>Overview</h3>

This project demonstrates how to use Ansible to automate the creation of an AWS EC2 instance
and the installation of an Apache web server on it. With a single command, you can provision a new Ubuntu instance in 
AWS and have it ready with Apache running.

<h3>Prerequisites</h3>
<ol>
<li>An AWS account with the necessary permissions to create EC2 instances.</li>
<li>Ansible installed on your local machine.</li>
<li>AWS CLI configured with your credentials.</li>
<li>SSH key pair created and available for use.</li>
</ol>

<h3>Playbook Breakdown</h3>
<ol>
<li>Create EC2 Instance: Provisions an Ubuntu instance with a public IP address.</li>
<li>Wait for SSH: Ensures the instance is ready to accept SSH connections.</li>
<li>Install Python: Installs Python on the newly created instance (required for further Ansible operations).</li>
<li>Install Apache: Updates the package list and installs Apache, ensuring the web server is running.</li>
</ol>

  <h4>Verify Installation</h4>
After the playbook completes, you can verify that Apache is running by accessing the public IP address of the EC2 instance in your web browser.

<h3>License</h3>
This project is licensed under the MIT License. See the LICENSE file for more details.
