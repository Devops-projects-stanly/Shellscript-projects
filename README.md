AWS Resource Lister Script Documentation

Description: This script automates the process of listing all resources in an AWS account for various services. It supports multiple AWS services and provides a command-line interface for users to specify the AWS region and the service they are interested in. The script retrieves and displays the resources for the specified service in the given region.

Usage: ./aws_resource_list.sh <aws_region> <aws_service>

Example: ./aws_resource_list.sh us-east-1 ec2

Script Workflow:

1.Check Arguments: The script checks if the required number of arguments (AWS region and service) are passed. If not, it displays the usage instructions and exits.

2.Assign Arguments: The script assigns the arguments to variables aws_region and aws_service, and converts the service name to lowercase.

3.Check AWS CLI Installation: The script checks if the AWS CLI is installed. If not, it prompts the user to install the AWS CLI and exits.

4.Check AWS CLI Configuration: The script checks if the AWS CLI is configured. If not, it prompts the user to configure the AWS CLI and exits.

5.List Resources: Based on the specified service, the script lists the resources in the specified AWS region using the appropriate AWS CLI command.

Error Handling:

* If the required arguments are not provided, the script displays usage instructions and exits.
* If the AWS CLI is not installed, the script prompts the user to install it and exits.
* If the AWS CLI is not configured, the script prompts the user to configure it and exits.
* If an unsupported AWS service is specified, the script displays an error message and exits.
