three Infrastructure as Code tools:
Terraform, Pulumi, and Bicep — and use each one to deploy resources from inside VS Code.

Terraform will deploy a VM in AWS

Pulumi (with Python) will create an S3 bucket

And Bicep will deploy a VM in Azure

🧰 Before we jump into the code, let’s set up the environment step-by-step.

✅ Step 1 – Install the CLI tools

 Install Terraform from terraform.io

 Install Azure CLI from aka.ms/installazurecli

 Install Pulumi from pulumi.com

✅ Step 2 – Install Python (for Pulumi)

Download Python from python.org

Make sure to check the box: "Add Python to PATH"

✅ Step 3 – Verify your tools are accessible Open a new terminal in VS Code and run:

bash
Copy
Edit
terraform -v
az version
pulumi version
python --version
If any of these return "not found", make sure they are added to your system PATH.

✅ Step 4 – Login to cloud providers

Run aws configure to set up your AWS credentials

Run az login to authenticate with Azure

For Pulumi, run pulumi login and select local or cloud backend
