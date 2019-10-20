This is the repo for the Managing infrastructure as code with Terraform, Cloud Build, and GitOps tutorial. This tutorial explains how to manage infrastructure as code with Terraform and Cloud Build using the popular GitOps methodology.

Configuring your dev environment
Just for demostration, this step will:

Configure an apache2 http server on network 'dev' and subnet 'dev-subnet-01'
Open port 80 on firewall for this http server
cd ../environments/dev
terraform init
terraform plan
terraform apply
terraform destroy
Promoting your environment to production
Once you have tested your app (in this example an apache2 http server), you can promote your configuration to prodution. This step will:

Configure an apache2 http server on network 'prod' and subnet 'prod-subnet-01'
Open port 80 on firewall for this http server
cd ../prod
terraform init
terraform plan
terraform apply
terraform destroy