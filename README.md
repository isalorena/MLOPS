# DVC Class 1

This repository refers to practical class of DVC of the MLOPS discipline

# How to run this project

## Dependencies

- Install [conda](https://www.anaconda.com/download) and run the following commands:

``` 
conda create --name mlops python=3.9
conda activate mlops
pip install -r requirements.txt
```
- Request the Client ID and Client Secret Key from the project administrator, and connect to Google Drive using dvc remote

``` 
dvc remote modify --local gdrive gdrive_client_id '<Client ID>'
dvc remote modify --local gdrive gdrive_client_secret '<Client Secret Key>'
```
## Storing files with DVC

- Adding a folder with files to be committed:

``` 
dvc add <Folder Name>
```
- Pushing to the remote repository for storage:

``` 
dvc push
```
