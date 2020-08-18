# Python - quick notes

## date-time
* `date.strftime(<date format>)` -> date to string
* `datetime.strptime(date_str, <date format>)` -> str to date

See also:
* https://strftime.org/


## NNs

| Problem                                 | Activation  | Loss                     |
|-----------------------------------------|-------------|--------------------------|
| Binary classification                   | sigmoid     | Binary crossentropy      |
| Multiclass, single-label classification | softmax     | Categoric crossentropy   |
| Multiclass, multilabel classification   | sigmoid     | Binary crossentropy      |
| Regression                              | none        | MSE                      |
| Regression to 0-1 (1 node)              | signoid     | MSE/binary cross entropy |


## regex
* `$`: match end.
* `^`: match start.

See also: 
* https://pythex.org/
* https://regexr.com/
* https://www.regular-expressions.info/tutorial.html 

## Django
* `django-admin startproject <my-project-name>`
* `python manage.py startapp <my-app-name>`
* `python manage.py shell`
* `python manage.py runserver`
* `python manage.py makemigrations`
* `python manage.py migrate`
* `python manage.py createsuperuser`
* `python manage.py check --deploy`


## Azure blobs
See https://docs.microsoft.com/en-us/python/api/azure-storage-blob/azure.storage.blob.blobserviceclient?view=azure-python

* `pip install azure-storage-blob`
* `blob_service_client = BlobServiceClient.from_connection_string(con_str)`: create blob client
* `blob_service_client.create_container(container_name)`: raises `ResourceExistsError` if container exists.
* `blob_service_client.list_containers()`: generator of existing containers.
* `container_client = blob_service_client.get_container_client('mycontainer')`: container-client instance
* `container_client.list_blobs()`: generator of existing blobs.
* `blob_client = container_client.get_blob_client(blob=filename)`: starting from container_client
* `blob_client = blob_service_client.get_blob_client(container=container_name, blob=filename)`: starting from blob_service_client
* Upload locally saved blob. Will raise `ResourceExistsError` if already exists.
```
with open(myfile, 'rb') as f:
  blob_client.upload_blob(f)
  
# to remove blob (see also docs)  
blob_client.delete_blob()  
```


