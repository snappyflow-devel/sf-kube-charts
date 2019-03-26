# Development of Helm Charts and using Github Repository are Helm Repo for SnappyFLow

## Steps
 - Create a new directory and copy all Helm chart related files under this directory
 - Build a tar.gz file for the directory.
 - Add this tar.gz file to index.yaml.
 - Commit the files to git hub repository.


### Commands to convert git repository as helm repository
 ```
 $ git clone <repo_url>
 $ cd <repo_name>
 $ helm package <chart_dir_path>  # build the tar.gz file
 $ helm repo index .         # create/update the index.yaml for repo
 $ git add .
 $ git commit -m '<commit message>'
 $ git push
 ```
 
###  How to use the git repo in SnappyFlow.
 - Go to Manage-> CI/CD settings.
 - Go to Chart Repository
 - Add your github repository.
