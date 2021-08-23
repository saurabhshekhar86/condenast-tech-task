# condenast-tech-task
Created a ci/cd pipeline
  Step1: Developer updating the code in github. Webhook is configured for the github repository, which triggers the pipeline
  Step2: the code will be built using maven - build automation tool
  Step3: the built code will be stored in build artifactory - sonatype nexus
  Step4: Ansible script would get this build and deploy in testing env using Tomcat container
  Step5: Quality check validation configured
  Step6: Once all the jobs are successful, then only code to be deployed in Production
  
  Note: Terraform is used to provision the AWS infrastructure
  
