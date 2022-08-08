# Jupyter, Python, Pandas, S3, Parquet, Redshift

The examples demonatrates:  
1️⃣ Querying Parquet file from S3 using AwsWrangler.  
2️⃣ Querying from Redshift tables using Glue & AwsWrangler. 

**Topics**
<table>
  <tr>
    <td>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png" width="30"/>
    </td>
    <td>
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT01Ctpf3nRjz7b9l-om2h2llNA0jL4d_MVtXXXHVF5mWIn5nyMXLgzYscFGZdbhf_LN8M&usqp=CAU" width="30"/>
    </td>
    <td>
    <img src="https://www.seekpng.com/png/small/410-4104604_here-is-how-to-add-a-shortcut-of.png" width="30"/>
    </td>
    <td>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/Amazon-S3-Logo.svg/1200px-Amazon-S3-Logo.svg.png" width="30"/>
    </td>
    <td>
    <img src="https://i0.wp.com/blog.contactsunny.com/wp-content/uploads/2020/04/parquet_logo.jpeg" width="30"/>
    </td>
    <td>
    <img src="https://www.clipartmax.com/png/middle/200-2001778_redshift-amazon-redshift-logo.png" width="30"/>
    </td>
  </tr>
</table>

## Requirements

- **AWS Account:** To create and use AWS services, you need to create an AWS account.
- **AWS Credentials:** In order to manage your services from command line tools, you need an **aws_access_key_id** and **an aws_secret_access_key**. Creating a new user for IaC purposes is recommended. For this, you can create a new user with **IAM**. For this;

  1. Go to IAM
  2. Under Users click 'Add User'
  3. Give a. username (like terraform_user)
  4. For credential type select 'Access key - Programmatic access' and click next
  5. Click 'Create Group', specify a group name and select 'AdministratorAccess' policy.
  6. Click Review and create user. This user has a programmatic access and admin permissions.

  After you create the user, go to Users and select the user you have created. Go to 'Security Credentials' and click 'Create access key'. This will give an access key id and a secret access key. Save and dont share these credentials. You can not see access key again after you close this window.
- **Make Redshift Cluster Public:** (at your own risk) https://aws.amazon.com/premiumsupport/knowledge-center/redshift-cluster-private-public/
