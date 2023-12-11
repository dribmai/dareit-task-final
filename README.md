# cloud_challenge - task_8

> This task covers setting up a static website stored in a bucket in GCP. All resources are deployed by using terraform and the deplyoment is automated using CI/CD pipeline via Github Actions.

<br>


### Solution:

1. Create w GCP account with a Service Account for terraform<br>
2. Generate a private key and save json file<br>
3. Create a bucket where the terraform file will be stored<br>
4. Create a new repository in Github and add a secret GCP key credentials to Actions<br>
5. Create your static website<br>
6. Create backend.tf (describes the bucket where the terraform file will be stored), provider.tf (defines provider for all the resources) and main.tf (describes what kind of resources will be created) files needed to obtain neccessary resources in GCP<br>
7. Create a file .github/workflow/terraform.yml to define CI/CD pipeline which will be triggering terraform actions with every push to the repository<br>
8. Commit all the files and check the Actions tab in your repo<br>